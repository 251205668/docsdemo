## 中后台学习

### 页面的主要路由分析

![1591325371527](C:\Users\努力中的杨先生\AppData\Roaming\Typora\typora-user-images\1591325371527.png)

> 全局是一个大的容器，`APP.vue`,然后显示的组件时`layout`,`layout`组件的构成
>
> - slide-bar
>
> - header
>
> - app-main 其中`app-main`也是一个容器，承载页面的主要内容,用`router-view`显示子路由
>
>   ```js
>   {
>       path: '/',
>       component: Layout,
>       redirect: '/dashboard',
>       children: [{
>         path: 'dashboard',
>         name: 'Dashboard',
>         component: () => import('@/views/dashboard/index'),
>         meta: { title: 'Dashboard', icon: 'dashboard' }
>       }]
>     },
>   ```
>
>   可以看出,`layout`组件的`app-main`就是主要内容

### 添加一个页面

```js
{
  path: '/excel',
  component: Layout,
  redirect: '/excel/export-excel',
  name: 'excel',
  meta: {
    title: 'excel',
    icon: 'excel'
  },
  children: [
    {
      path: 'export-excel',
      component: ()=>import('excel/exportExcel'),
      name: 'exportExcel',
      meta: { title: 'exportExcel' }
    }
  ]
}
```



### 权限校验

**生成权限菜单**

在`async-router`上配置路由元信息,增加`roles`属性

```js
{
    path:'/student',
    component:layout,
    redirect:'/student/add',
    meta:{title:'学生管理',icon:'documation',roles=['admin']}
    children:[
        {
            path:'/create',
            component:()=>important('')
            name
        }
    ]
}
```

### 修改配置代理接口

首先关闭`mock数据`

注释以下代码

`main.js`

```js
 if (process.env.NODE_ENV === 'production') {
  const { mockXHR } = require('../mock')   
  mockXHR()
 }
```

`vue.config.js`

```js
devServer
```

更改`axios`的`baseUrl`

```js
修改环境配置文件 全局变量
```



### 登录源码分析

```js
handleLogin() {
  this.$refs.loginForm.validate(valid => {
    if (valid) {
        // 通过校验
      this.loading = true
       // 提交表单数据 提交一个vuex的commit，因为用了namespaced = true 所以要加上namespace
      this.$store.dispatch('user/login', this.loginForm)
        .then(() => {
          // 保存token之后 如果有redirect就前往redirect 默认到达根路径
          this.$router.push({ path: this.redirect || '/', query: this.otherQuery })
          this.loading = false
        })
        .catch(() => {
          // 捕获异常
          this.loading = false
        })
    } else {
      console.log('error submit!!')
      return false
    }
  })
}
```

`vuex`中的`user`

```js

// 动作定义 异步操作 需要更改多个state
const actions = {
  // 用户登陆
  login({ commit }, userInfo) {
    const { username, password } = userInfo
    // 返回promise对象
    return new Promise((resolve, reject) => {
      login({ username: username.trim(), password: password }).then(response => {
        const { data } = response
        // 设置vuex数据和保存cookie
        commit('SET_TOKEN', data.token)
        setToken(data.token)
        resolve()
      }).catch(error => {
        reject(error)
      })
    })
  },

  // 获取用户信息
  getInfo({ commit, state }) {
    return new Promise((resolve, reject) => {
      // 携带token信息请求用户信息
      getInfo(state.token).then(response => {
        const { data } = response
        const { roles, name, avatar } = data
        // 返回信息 roles是必须的
        if (!roles || roles.length <= 0) {
          reject('getInfo: roles must be a non-null array!')
        }
        // 保存vuex数据
        commit('SET_ROLES', roles)
        commit('SET_NAME', name)
        commit('SET_AVATAR', avatar)
        resolve(data)
      }).catch(error => {
        reject(error)
      })
    })
  },

  // 用户退出登录
  logout({ commit, state }) {
    return new Promise((resolve, reject) => {
      // 退出登录
      try {
        // 将cookie中的token清除
        removeToken()
        // 路由重定向
        resetRouter()
        // vuex信息清除
        commit('RESET_STATE')
        resolve()
      } catch (error) {
        reject(error)
      }
    })
  },
  // remove token
  resetToken({ commit }) {
    return new Promise(resolve => {
      removeToken() // must remove  token  first
      commit('RESET_STATE')
      resolve()
    })
  }
}

export default {
  namespaced: true,
  state,
  mutations,
  actions
}


```

分析:

> 登录分为几步操作
>
> 1. 校验表单，提交数据
> 2. 执行`vuex`的commit，请求服务端数据然后保存`token`到`cookie`和`vuex`当中，返回`promise·resolve`
> 3. 请求导数据后路由重定向到`redirect`，如果没有就重定向到`/`
>
> 获取用户信息
>
>         1.  携带`token`请求接口
>         2.  获取`roles`，`avatar`,`name`，其中`roles`必须存在
>         3.  保存数据在`vuex`
>
> 退出登录
>
>          1.  清除`cookie`中的数据
>          2.  将`vuex`用户信息置空
>          3.  路由重定向，此时不携带`token`，路由会定位到`login`

其中这两个接口返回的数据相对固定

- 登录

  ```json
  {
      "data":{
          token:""
      }
  }
  ```

  

- 获取用户信息

  ```json
  {
      "data":{
          avatar:"",
          name:"",
          roles:['admin'...]
      }
  }
  ```

  

### 框架的路由权限分析

![](https://image.yangxiansheng.top/img/login_process.png?imagelist)

访问路由时会从 Cookie 中获取 Token，判断 Token 是否存在：

- 如果 Token 存在，将根据用户角色生成动态路由，然后访问路由，生成对应的页面组件。这里有一个特例，即用户访问 `/login` 时会重定向至 `/` 路由；
- 如果 Token 不存在，则会判断路由是否在白名单中，如果在白名单中将直接访问，否则说明该路由需要登录才能访问，此时会将路由生成一个 redirect 参数传入 login 组件，实际访问的路由为：`/login?redirect=/xxx`。

```js
router.beforeEach(async(to, from, next) => {
  // 启动进度条
  NProgress.start()
  // 修改页面标题
  document.title = getPageTitle(to.meta.title)
  // 从 Cookie 获取 Token
  const hasToken = getToken()
  
  // 判断 Token 是否存在
  if (hasToken) {
    // 如果当前路径为 login 则直接重定向至首页
    if (to.path === '/login') {
      next({ path: '/' })
      NProgress.done()
    } else {
      // 判断用户的角色是否存在
      const hasRoles = store.getters.roles && store.getters.roles.length > 0
      // 如果用户角色存在，则直接访问
      if (hasRoles) {
        next()
      } else {
       
          try {
          // 异步获取用户的角色
          const { roles } = await store.dispatch('user/getInfo')
          //! 根据用户角色，动态生成路由
          const accessRoutes = await store.dispatch('permission/generateRoutes', roles)
          // 调用 router.addRoutes 动态添加路由
          router.addRoutes(accessRoutes)
          // 使用 replace 访问路由，不会在 history 中留下记录
          next({ ...to, replace: true })
        } catch (error) {
          // 移除 Token 数据
          await store.dispatch('user/resetToken')
          // 显示错误提示
          Message.error(error || 'Has Error')
          // 重定向至登录页面
          next(`/login?redirect=${to.path}`)
          NProgress.done()
        }
      }
    }
  } 
    else {
    // 如果访问的 URL 在白名单中，则直接访问
    if (whiteList.indexOf(to.path) !== -1) {
      next()
    } else {
      // 如果访问的 URL 不在白名单中，则直接重定向到登录页面，并将访问的 URL 添加到 redirect 参数中
      next(`/login?redirect=${to.path}`)
      NProgress.done()
    }
  }
})

router.afterEach(() => {
  // 停止进度条
  NProgress.done()
})
```



## 图表

### 折线图

```js
<template>
  <div class="chart" style="width:100%;height:350px"  />
</template>

<script>
import echarts from 'echarts'
require('echarts/theme/macarons') // echarts theme
import resize from './mixins/resize'

export default {
  mixins: [resize],
  data() {
    return {
      chart: null
    }
  },
  mounted() {
    this.$nextTick(() => {
      this.initChart()
    })
  },
    // 组件销毁 清空图表提高性能
  beforeDestroy() {
    if (!this.chart) {
      return
    }
    this.chart.dispose()
    this.chart = null
  },
  methods: {
      // 初始化图表
    initChart() {
      this.chart = echarts.init(this.$el, 'macarons')
      this.setOptions(this.chartData)
    },
      // 配置项
     //  expectedData: [100, 120, 161, 134, 105, 160, 165],
    //   actualData: [120, 82, 91, 154, 162, 140, 145]
    setOptions({ expectedData, actualData } = {}) {
      this.chart.setOption({
         // x轴
        xAxis: {
          data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
          // 不显示标尺
          boundaryGap: false,
          axisTick: {
            show: false
          }
        },
         // 网格分布
        grid: {
          left: 10,
          right: 10,
          bottom: 20,
          top: 30,
          containLabel: true
        },
         // 提示信息
        tooltip: {
          trigger: 'axis',
          axisPointer: {
            type: 'cross'
          },
          padding: [5, 10]
        },
        yAxis: {
          axisTick: {
            show: false
          }
        },
         // 点击可切换折线图显示的选项
        legend: {
          data: ['expected', 'actual']
        },
         // 数据配置
        series: [{
          name: 'expected', itemStyle: {
             // 拐点颜色和线颜色
            normal: {
              color: '#FF005A',
              lineStyle: {
                color: '#FF005A',
                width: 2
              }
            }
          },
          smooth: true,
          type: 'line',
          data: expectedData,
          animationDuration: 2800,
          animationEasing: 'cubicInOut'
        },
        {
          name: 'actual',
          smooth: true,
          type: 'line',
          itemStyle: {
            normal: {
              color: '#3888fa',
              lineStyle: {
                color: '#3888fa',
                width: 2
              },
              areaStyle: {
                color: '#f3f8ff'
              }
            }
          },
          data: actualData,
          animationDuration: 2800,
          animationEasing: 'quadraticOut'
        }]
      })
    }
  }
}
</script>

```



### 饼图

```js
<template>
  <div class="chart" style="width:100%;height:550px" />
</template>

<script>
import echarts from 'echarts'
require('echarts/theme/macarons') // echarts theme
import resize from '@/utils/resize'
export default {
  name: '',
  components: {},
  mixins: [resize],
  props: {
    pipeData: {
      type: Array,
      default: () => {
        return []
      }
    }
  },
  data() {
    return {

    }
  },

  computed: {},

  watch: {},
  created() {},

  beforeMount() {},

  mounted() {
    this.initChart()
  },
  beforeDestroy() {
    if (!this.chart) {
      return
    }
    this.chart.dispose()
    this.chart = null
  },

  methods: {
    // 初始化图表
    initChart() {
      setTimeout(() => {
        this.chart = echarts.init(this.$el, 'macarons')
        this.setOptions()
      }, 500)
    },
    setOptions() {
      this.chart.setOption({
        title: {
          text: '学生课程分数情况图',
          subtext: '仅供参考',
          left: 'center'
        },
        // 配置提示
        tooltip: {
          trigger: 'item',
          formatter: '{a} <br/>{b} : {c} ({d}%)'
        },
        // 选项卡配置
        legend: {
          // horizontal为横轴
          orient: 'veritcal',
          // 图例组件离容器左侧的距离
          left: 70,
          top: 40,
          data: ['60-70分课程数', '70-80分课程数', '80-90分课程数', '90-100分课程数', '不及格课程数']
        },
        series: [
          {
            name: '课程分布情况',
            type: 'pie',
            radius: '55%',
            center: ['50%', '60%'],
            data: [
              { value: this.pipeData[1], name: '60-70分课程数' },
              { value: this.pipeData[2], name: '70-80分课程数' },
              { value: this.pipeData[3], name: '80-90分课程数' },
              { value: this.pipeData[4], name: '90-100分课程数' },
              { value: this.pipeData[0], name: '不及格课程数' }
            ],
            emphasis: {
              itemStyle: {
                shadowBlur: 10,
                shadowOffsetX: 0,
                shadowColor: 'rgba(0, 0, 0, 0.5)'
              }
            }
          }
        ]
      })
    }
  }

}

</script>
<style lang='scss' scoped>

</style>

```

![1591965732372](C:\Users\努力中的杨先生\AppData\Roaming\Typora\typora-user-images\1591965732372.png)

## 表格

### 无边框表格

```html
  <el-table
        :data="userInfo.course_list"
        fit
        highlight-current-row
        style="box-sizing:border-box;width: 100%;padding-top:15px;margin-left:40px; box-shadow: 0 2px 4px rgba(0, 0, 0, .12), 0 0 6px rgba(0, 0, 0, .04);"
      >
        <el-table-column label="序号" type="index" align="center" width="90" />
        <el-table-column label="课程编号" prop="cno" align="center" width="90">
          <template slot-scope="scope">
            <span style="color:#409EFF;font-size:17px;font-weight:500">{{ scope.row.cno }}</span>
          </template>
        </el-table-column>
        <el-table-column label="课程名" prop="cno" align="center" min-width="200">
          <template slot-scope="scope">
            <span style="color:#606266;font-size:16px;line-height:23px;font-weight:500">{{ scope.row.course_detail[0].name }}</span>
          </template>
        </el-table-column>
        <el-table-column label="学分" prop="cno" align="center" width="90">
          <template slot-scope="scope">
            <span style="color:#409EFF;font-size:17px;font-weight:500">{{ scope.row.course_detail[0].credit }}</span>
          </template>
        </el-table-column>
        <el-table-column label="学时" prop="cno" align="center" width="90">
          <template slot-scope="scope">
            <span style="color:#909399;font-size:17px;font-weight:500">{{ scope.row.course_detail[0].period }}</span>
          </template>
        </el-table-column>
        <el-table-column label="学期" align="center" width="200">
          <template slot-scope="{row}">
            <el-tag v-if="row.course_detail[0].term !== '第二学期'" type="danger">{{ row.course_detail[0].term }}</el-tag>
            <el-tag v-if=" row.course_detail[0].term=== '第二学期'" type="success">{{ row.course_detail[0].term }}</el-tag>
          </template>
        </el-table-column>
      </el-table>
```

具体配置参考`element-ui`文档

### 有边框文档

```html
   <el-table
        v-loading="listLoading"
        :data="list"
        border
        fit
        highlight-current-row
        style="width: 100%;"
      >
        <el-table-column label="序号" type="index" align="center" width="100" />
        <el-table-column label="课程编号" prop="cno" align="center" width="100">
          <template slot-scope="scope">
            <span style="color:#409EFF;font-size:17px;font-weight:500">{{ scope.row.cno }}</span>
          </template>
        </el-table-column>
        <el-table-column label="课程名" prop="course_detail[0].name" align="center" width="130">
          <template slot-scope="scope">
            <span>{{ scope.row.course_detail[0].name }}</span>
          </template>
        </el-table-column>
        <el-table-column label="学分" prop="course_detail[0].credit" align="center" width="100">
          <template slot-scope="scope">
            <span style="color:#E6A23C;font-size:17px;font-weight:500">{{ scope.row.course_detail[0].credit }}</span>
          </template>
        </el-table-column>
        <el-table-column label="学期" prop="course_detail[0].term" align="center" width="150">
          <template slot-scope="scope">
            <span>{{ scope.row.course_detail[0].term }}</span>
          </template>
        </el-table-column>
        <el-table-column label="学时" prop="course_detail[0].period" align="center" width="100">
          <template slot-scope="scope">
            <span style="color:#67C23A;font-size:17px;font-weight:500">{{ scope.row.course_detail[0].period }}</span>
          </template>
        </el-table-column>
        <el-table-column label="封面图" prop="course_detail[0].img" align="center" width="199">
          <template slot-scope="scope">
            <img width="80px" height="80px" :src="scope.row.course_detail[0].img" alt="">
          </template>
        </el-table-column>
        <el-table-column label="成绩" prop="score" align="center" width="100">
          <template slot-scope="scope">
            <span style="color:#F56C6C;font-size:17px;font-weight:500">{{ scope.row.score }}</span>
          </template>
        </el-table-column>

        <el-table-column label="操作" align="center" width="290" class-name="small-padding fixed-width">
          <template slot-scope="{row}">
            <el-button disabled type="primary" size="mini" @click="confirmEdit(row)">
              编辑
            </el-button>
            <el-button disabled size="small" type="success">
              添加
            </el-button>
            <el-button disabled size="small" type="danger">
              删除
            </el-button>
          </template>
        </el-table-column>
      </el-table>
```

### 综合表格

```vue
<div class="app-container">
    <div class="filter-container">
      <el-input v-model="listQuery.title" :placeholder="$t('table.title')" style="width: 200px;" class="filter-item" @keyup.enter.native="handleFilter" />
      <el-select v-model="listQuery.importance" :placeholder="$t('table.importance')" clearable style="width: 90px" class="filter-item">
        <el-option v-for="item in importanceOptions" :key="item" :label="item" :value="item" />
      </el-select>
      <el-select v-model="listQuery.type" :placeholder="$t('table.type')" clearable class="filter-item" style="width: 130px">
        <el-option v-for="item in calendarTypeOptions" :key="item.key" :label="item.display_name+'('+item.key+')'" :value="item.key" />
      </el-select>
      <el-select v-model="listQuery.sort" style="width: 140px" class="filter-item" @change="handleFilter">
        <el-option v-for="item in sortOptions" :key="item.key" :label="item.label" :value="item.key" />
      </el-select>
      <el-button v-waves class="filter-item" type="primary" icon="el-icon-search" @click="handleFilter">
        {{ $t('table.search') }}
      </el-button>
      <el-button class="filter-item" style="margin-left: 10px;" type="primary" icon="el-icon-edit" @click="handleCreate">
        {{ $t('table.add') }}
      </el-button>
      <el-button v-waves :loading="downloadLoading" class="filter-item" type="primary" icon="el-icon-download" @click="handleDownload">
        {{ $t('table.export') }}
      </el-button>
      <el-checkbox v-model="showReviewer" class="filter-item" style="margin-left:15px;" @change="tableKey=tableKey+1">
        {{ $t('table.reviewer') }}
      </el-checkbox>
    </div>

    <el-table
      :key="tableKey"
      v-loading="listLoading"
      :data="list"
      border
      fit
      highlight-current-row
      style="width: 100%;"
      @sort-change="sortChange"
    >
      <el-table-column :label="$t('table.id')" prop="id" sortable="custom" align="center" width="80" :class-name="getSortClass('id')">
        <template slot-scope="scope">
          <span>{{ scope.row.id }}</span>
        </template>
      </el-table-column>
      <el-table-column :label="$t('table.date')" width="150px" align="center">
        <template slot-scope="scope">
          <span>{{ scope.row.timestamp | parseTime('{y}-{m}-{d} {h}:{i}') }}</span>
        </template>
      </el-table-column>
      <el-table-column :label="$t('table.title')" min-width="150px">
        <template slot-scope="{row}">
          <span class="link-type" @click="handleUpdate(row)">{{ row.title }}</span>
          <el-tag>{{ row.type | typeFilter }}</el-tag>
        </template>
      </el-table-column>
      <el-table-column :label="$t('table.author')" width="110px" align="center">
        <template slot-scope="scope">
          <span>{{ scope.row.author }}</span>
        </template>
      </el-table-column>
      <el-table-column v-if="showReviewer" :label="$t('table.reviewer')" width="110px" align="center">
        <template slot-scope="scope">
          <span style="color:red;">{{ scope.row.reviewer }}</span>
        </template>
      </el-table-column>
      <el-table-column :label="$t('table.importance')" width="80px">
        <template slot-scope="scope">
          <svg-icon v-for="n in +scope.row.importance" :key="n" icon-class="star" class="meta-item__icon" />
        </template>
      </el-table-column>
      <el-table-column :label="$t('table.readings')" align="center" width="95">
        <template slot-scope="{row}">
          <span v-if="row.pageviews" class="link-type" @click="handleFetchPv(row.pageviews)">{{ row.pageviews }}</span>
          <span v-else>0</span>
        </template>
      </el-table-column>
      <el-table-column :label="$t('table.status')" class-name="status-col" width="100">
        <template slot-scope="{row}">
          <el-tag :type="row.status | statusFilter">
            {{ row.status }}
          </el-tag>
        </template>
      </el-table-column>
      <el-table-column :label="$t('table.actions')" align="center" width="230" class-name="small-padding fixed-width">
        <template slot-scope="{row}">
          <el-button type="primary" size="mini" @click="handleUpdate(row)">
            {{ $t('table.edit') }}
          </el-button>
          <el-button v-if="row.status!='published'" size="mini" type="success" @click="handleModifyStatus(row,'published')">
            {{ $t('table.publish') }}
          </el-button>
          <el-button v-if="row.status!='draft'" size="mini" @click="handleModifyStatus(row,'draft')">
            {{ $t('table.draft') }}
          </el-button>
          <el-button v-if="row.status!='deleted'" size="mini" type="danger" @click="handleModifyStatus(row,'deleted')">
            {{ $t('table.delete') }}
          </el-button>
        </template>
      </el-table-column>
    </el-table>

    <pagination v-show="total>0" :total="total" :page.sync="listQuery.page" :limit.sync="listQuery.limit" @pagination="getList" />

    <el-dialog :title="textMap[dialogStatus]" :visible.sync="dialogFormVisible">
      <el-form ref="dataForm" :rules="rules" :model="temp" label-position="left" label-width="70px" style="width: 400px; margin-left:50px;">
        <el-form-item :label="$t('table.type')" prop="type">
          <el-select v-model="temp.type" class="filter-item" placeholder="Please select">
            <el-option v-for="item in calendarTypeOptions" :key="item.key" :label="item.display_name" :value="item.key" />
          </el-select>
        </el-form-item>
        <el-form-item :label="$t('table.date')" prop="timestamp">
          <el-date-picker v-model="temp.timestamp" type="datetime" placeholder="Please pick a date" />
        </el-form-item>
        <el-form-item :label="$t('table.title')" prop="title">
          <el-input v-model="temp.title" />
        </el-form-item>
        <el-form-item :label="$t('table.status')">
          <el-select v-model="temp.status" class="filter-item" placeholder="Please select">
            <el-option v-for="item in statusOptions" :key="item" :label="item" :value="item" />
          </el-select>
        </el-form-item>
        <el-form-item :label="$t('table.importance')">
          <el-rate v-model="temp.importance" :colors="['#99A9BF', '#F7BA2A', '#FF9900']" :max="3" style="margin-top:8px;" />
        </el-form-item>
        <el-form-item :label="$t('table.remark')">
          <el-input v-model="temp.remark" :autosize="{ minRows: 2, maxRows: 4}" type="textarea" placeholder="Please input" />
        </el-form-item>
      </el-form>
      <div slot="footer" class="dialog-footer">
        <el-button @click="dialogFormVisible = false">
          {{ $t('table.cancel') }}
        </el-button>
        <el-button type="primary" @click="dialogStatus==='create'?createData():updateData()">
          {{ $t('table.confirm') }}
        </el-button>
      </div>
    </el-dialog>

    <el-dialog :visible.sync="dialogPvVisible" title="Reading statistics">
      <el-table :data="pvData" border fit highlight-current-row style="width: 100%">
        <el-table-column prop="key" label="Channel" />
        <el-table-column prop="pv" label="Pv" />
      </el-table>
      <span slot="footer" class="dialog-footer">
        <el-button type="primary" @click="dialogPvVisible = false">{{ $t('table.confirm') }}</el-button>
      </span>
    </el-dialog>
  </div>
```



### 导出Excel表格

引入`vue-element-admin`提供的导出`js`文件

```js
handleDownload() {
      this.downLoading = true
  import('@/vendor/export2Excel').then(excel => {
    // 设置表头
    const tHeader = ['课程编号', '课程名', '学分', '学期', '学时', '成绩']
    // 选择导出到表的字段
    const filterVal = ['cno', 'name', 'credit', 'term', 'period', 'score']
    const data = this.formatJson(filterVal, this.list)
    excel.export_json_to_excel({
      header: tHeader,
      data,
      filename: '成绩单'
    })
    this.downLoading = false
  })
   },
  // 将对象数组对应fileterval的字段取出 返回一个数组     
   formatJson(filterval, data) {
      // 遍历json数据
      return data.map(v => filterval.map(item => {
        if (item === 'cno' || item === 'score') {
          return v[item]
        } else {
          const course_detail = v.course_detail[0]
          return course_detail[item]
        }
      }))
    }
```

## websocket

### 服务端

```js
const WebSocket = require('ws')
const http = require('http')
// 创建WebSocket服务
const wss = new WebSocket.Server({ noServer: true })
const server = http.createServer()

const group = {} // 记录每个房间号的人数

// 多聊天室功能
// roomid -> 对应相同的roomid进行广播消息
wss.on('connection', function connection(ws) {
  // ws代表当前收到消息的客户端

  // 接收客户端消息
  ws.on('message', function(msg) {
    console.log(msg) //msg: {"event":"enter","message":"1","roomid":"1"}
    // 转成对象
    const msgObj = JSON.parse(msg)

    // 进入房间
    if (msgObj.event === 'enter') {
      ws.name = msgObj.message
      ws.roomid = msgObj.roomid
      if (typeof group[ws.roomid] === 'undefined') {
        group[ws.roomid] = 1
      } else {
        group[ws.roomid] += 1
      }
    }

    // 广播消息(即获取所有的客户端)
    wss.clients.forEach(client => {
      // 补充：如何判断非自己的客户端：ws !== client
      if (client.readyState === WebSocket.OPEN && client.roomid === ws.roomid) {
        msgObj.name = ws.name
        // msgObj.num = wss.clients.size; // 聊天室的人数
        msgObj.num = group[ws.roomid] // 聊天室的人数
         // 发送回客户端在线人数和 消息
        client.send(JSON.stringify(msgObj))
      }
    })
  })

  // 当ws客户端断开链接的时候
  ws.on('close', function(msg) {
    if (ws.name) {
      group[ws.roomid] -= 1
    }

    const msgObj = {}
    wss.clients.forEach(client => {
      if (client.readyState === WebSocket.OPEN && ws.roomid === client.roomid) {
        msgObj.name = ws.name
        msgObj.num = group[ws.roomid] // 聊天室的人数
        msgObj.event = 'out'
        client.send(JSON.stringify(msgObj))
      }
    })
  })
})

server.on('upgrade', function upgrade(request, socket, head) {
  wss.handleUpgrade(request, socket, head, function done(ws) {
    wss.emit('connection', ws, request)
  })
})

server.listen(3000)

```

### 客户端

> 变量均用双向绑定定义

```js

        message: '',
        lists: [],
        ws: {},
        name: '',
        isShow: true,
        num: 0,
        roomid: "" //房间号
mounted(){
        this.ws = new WebSocket('ws://127.0.0.1:3000');
        this.ws.onopen = this.onOpen
        this.ws.onmessage = this.onMessage
        this.ws.onclose = this.onClose
        this.ws.onerror = this.onError
}


// 监听是否打开websocket
  onOpen: function () {
          console.log('open:' + this.ws.readyState);
        },

// 进入聊天室
          enter() {
            if(this.name.trim() === '') {
              alert('用户名不得为空')
              return
            }
            this.isShow = false
            this.ws.send(JSON.stringify({
              event: "enter",
              message: this.name,
              roomid: this.roomid
            }))
          },
 // 接收消息
  onMessage: function (event) {
          // 当用户未进入聊天室，则不接收消息
          if (this.isShow) {
            return
          }

          // 接收服务端发送过来的消息
          var tmp = JSON.parse(event.data)

          if (tmp.event === 'enter') {
            // 当有新用户进入聊天室  tmp.message为用户名
            this.lists.push('欢迎：' + tmp.message + '加入聊天室')
          } else if (tmp.event === 'out') {
            this.lists.push(tmp.name + '已经退出了聊天室!')
          } else {
            if (tmp.name !== this.name) { // 屏蔽发送给自己的消息
              // 接收正常的聊天
              this.lists.push(tmp.name + ':' + tmp.message)
            }
          }
          this.num = tmp.num
        },
    // 发送消息
        send: function () {
          // 客户端显示
          this.lists.push(this.name + ':' + this.message)
          this.ws.send(JSON.stringify({
            event: "message",
            message: this.message
          }))
          this.message = ''
        }
  

// 关闭和异常
   onClose: function () {
          // 当链接主动断开的时候触发close事件
          console.log('close:' + this.ws.readyState);
        },
        onError: function () {
          // 当连接失败的时候触发error事件
          console.log('error:' + this.ws.readyState);
        },

```





### 实例(服务端)

```js
const WebSocket = require('ws')
const http = require('http')
const wss = new WebSocket.Server({ noServer: true })
const server = http.createServer()
const group = {} // 记录每个房间号的人数
// 多聊天室功能
// roomid -> 对应相同的roomid进行广播消息
wss.on('connection', function connection(ws) {
  // ws代表当前收到消息的客户端
  // 接收客户端消息
  ws.on('message', function(msg) {
    const msgObj = JSON.parse(msg)
    if (msgObj.event === 'enter') {
      // 用户信息
      ws.name = msgObj.name
      ws.avatar = msgObj.avatar
      ws.roomid = msgObj.roomid
      // 首次进入房间判断 房间人数置为1
      if (typeof group[ws.roomid] === 'undefined') {
        group[ws.roomid] = 1
      } else {
        group[ws.roomid] += 1
      }
    }
    // 广播消息(即获取所有的客户端)
    wss.clients.forEach(client => {
      // 补充：如何判断非自己的客户端：ws !== client
      if (client.readyState === WebSocket.OPEN && client.roomid === ws.roomid) {
        // 同一个房间 进行广播
        msgObj.name = ws.name
        msgObj.avatar = ws.avatar
        // 房间人数
        msgObj.num = group[ws.roomid]
        // 发送广播消息 附带消息
        client.send(JSON.stringify(msgObj))
      }
    })
  })
  // 当ws客户端断开链接的时候
  ws.on('close', function(msg) {
    if (ws.name) {
      group[ws.roomid] -= 1
    }
    const msgObj = {}
    wss.clients.forEach(client => {
      if (client.readyState === WebSocket.OPEN && ws.roomid === client.roomid) {
        msgObj.name = ws.name
        msgObj.avatar = ws.avatar
        msgObj.num = group[ws.roomid] // 聊天室的人数
        msgObj.event = 'out'
        client.send(JSON.stringify(msgObj))
      }
    })
  })
})
server.on('upgrade', function upgrade(request, socket, head) {
  wss.handleUpgrade(request, socket, head, function done(ws) {
    wss.emit('connection', ws, request)
  })
})
server.listen(3000)

```

###  实例(客户端)

#### 监听开启websocket

```js
  mounted() {
    this.isShow = true
    this.ws = new WebSocket('ws://127.0.0.1:3000')
    this.ws.onopen = this.onOpen
    this.ws.onmessage = this.onMessage
    this.ws.onclose = this.onClose
    this.ws.onerror = this.onError
  },
  methods: {
    // 监听开启
    onOpen() {
      console.log('webSocket is open' + this.ws.readyState)
    }
  }
```



#### 监听进入房间

```js
 enter() {
      this.isShow = false
      // 发送消息 广播进入房间
      this.ws.send(JSON.stringify({
        event: 'enter',
        name: this.userInfo.name,
        avatar: this.userInfo.avatar,
        rootmid: this.roomid
      }))
    },
```



#### 监听传来的消息

```js
  // 接收信息
    onMessage(event) {
      // 服务端传递过来的数据
      if (this.isShow) {
        return
      }
      const data = JSON.parse(event.data)
      // 如果是进入或者退出房间
      const messageInfo = {}
      messageInfo.avatar = data.avatar
      messageInfo.roomNum = data.num
      messageInfo.name = data.name
      if (data.event === 'enter') {
        messageInfo.message = '加入房间'
      } else if (data.event === 'close') {
        messageInfo.message = '退出了房间'
      } else {
        messageInfo.message = data.message
      }
      this.lists.push(messageInfo)
      this.num = data.num
      this.message = ''
    },
```



#### 发送消息

```js
 // 发送消息
    send() {
      // this.lists.push()
      this.ws.send(JSON.stringify({
        event: 'message',
        message: this.message
      }))
    },
```



#### 监听错误或者推出

```js

    clear() {
      this.message = ''
    },
    // 监听关闭和异常
    onClose: function() {
      // 当链接主动断开的时候触发close事件
      console.log('close:' + this.ws.readyState)
    },
    onError: function() {
      // 当连接失败的时候触发error事件
      console.log('error:' + this.ws.readyState)
    }
  }
```

### 客户端完整代码

```vue
<template>
  <div class="container">
    <el-card v-if="!isShow" class="message-content">
      <p slot="header" style="padding:10px;max-height:2px!important;box-sizing:border-box;font-weight:800">在线聊天系统   在线人数:{{ num }}人</p>
      <el-alert
        center
        :title="time"
        type="info"
        :closable="false"
      />
      <div v-for="(item,index) of lists" ref="ms" :key="index" class="message">
        <el-alert
          v-if="item.message === '加入房间' && typeof(item.name) !== 'undefined'"
          center
          :title="item.name+item.message"
          style="margin-top:20px;"
          type="success"
          :closable="false"
        />
        <el-alert
          v-if="item.message === '加入房间'&& typeof(item.name) === 'undefined'"
          center
          :title="'超级管理员'+item.message"
          style="margin-top:20px;"
          type="error"
          :closable="false"
        />
        <div v-if="item.name !== userInfo.name && item.message!== '加入房间'" class="content-left">
          <img style="border-radius:6px" :src="item.avatar" alt="" width="40px" height="40px">
          <div class="info">
            <span class="name">{{ item.name }}</span>
            <span class="message-left" type="info">{{ item.message }}</span>
          </div>
        </div>
        <div v-if="item.name === userInfo.name && item.message !== '加入房间'" class="content-right">
          <div class="info">
            <!-- <span class="name">{{ item.name }}</span> -->
            <span class="message-right" type="primary">{{ item.message }}</span>
          </div>
          <img style="border-radius:6px" :src="item.avatar" alt="" width="40px" height="40px">
        </div>
      </div>
    </el-card>
    <div v-if="!isShow" class="message-input">
      <el-input
        v-model="message"
        type="textarea"
        :rows="6"
        placeholder="请输入内容"
      />
    </div>
    <div v-if="!isShow" class="send-wrapper">
      <el-button style="width:120px;border:none" @click="clear">取消</el-button>
      <el-button type="primary" style="width:120px; margin-left:15px" @click="send">发送</el-button>
    </div>
    <div class="enter-button">
      <el-button v-if="isShow" type="primary" @click="enter">进入聊天室</el-button>
    </div>
  </div>
</template>

<script>
import dayjs from 'dayjs'
import { mapGetters } from 'vuex'
export default {
  name: '',
  components: {},
  props: {},
  data() {
    return {
      message: '',
      lists: [],
      ws: {},
      isShow: true,
      num: 0,
      roomid: 1,
      time: dayjs().format('YYYY-MM-DD HH:mm:ss')
    }
  },
  computed: {
    ...mapGetters([
      'userInfo'
    ])
  },

  watch: {},
  created() {},

  beforeMount() {},

  mounted() {
    this.isShow = true
    this.ws = new WebSocket('ws://127.0.0.1:3000')
    this.ws.onopen = this.onOpen
    this.ws.onmessage = this.onMessage
    this.ws.onclose = this.onClose
    this.ws.onerror = this.onError
  },

  methods: {
    // 监听开启
    onOpen() {
      console.log('webSocket is open' + this.ws.readyState)
    },

    // 监听进入房间
    enter() {
      this.isShow = false
      // 发送消息 广播进入房间
      this.ws.send(JSON.stringify({
        event: 'enter',
        name: this.userInfo.name,
        avatar: this.userInfo.avatar,
        rootmid: this.roomid
      }))
    },

    // 接收信息
    onMessage(event) {
      // 服务端传递过来的数据
      if (this.isShow) {
        return
      }
      const data = JSON.parse(event.data)
      // 如果是进入或者退出房间
      const messageInfo = {}
      messageInfo.avatar = data.avatar
      messageInfo.roomNum = data.num
      messageInfo.name = data.name
      if (data.event === 'enter') {
        messageInfo.message = '加入房间'
      } else if (data.event === 'close') {
        messageInfo.message = '退出了房间'
      } else {
        messageInfo.message = data.message
      }
      this.lists.push(messageInfo)
      this.num = data.num
      this.message = ''
    },

    // 发送消息
    send() {
      // this.lists.push()
      this.ws.send(JSON.stringify({
        event: 'message',
        message: this.message
      }))
    },
    clear() 
      this.message = ''
    },
    // 监听关闭和异常
    onClose: function() {
      // 当链接主动断开的时候触发close事件
      console.log('close:' + this.ws.readyState)
    },
    onError: function() {
      // 当连接失败的时候触发error事件
      console.log('error:' + this.ws.readyState)
    }
  }

}
```

