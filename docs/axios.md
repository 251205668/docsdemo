# axios

## `GET`

```js
Axios.get('http://localhost:3000/v1/public/getlist',{
  headers:{
    'Content-Type':'application/json',
    'Authorization':'Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI1ZWQzZGEzMDVkMDc4NjdjZjg4N2RhY2IiLCJpYXQiOjE1OTEwOTUxNjEsImV4cCI6MTU5MTI2Nzk2MX0.m4DLxbhchw3lpOQf8vY_1R985y9zPds_2kK1xnGVRxA'
  },
  params:{
    category:'音乐'

  }
},).then((res)=>{
  console.log(res.data.data)
  console.log(res.config)
})



axios({
  method:"GET",
  headers:{
    "Content-Type":"application/json",
    "Authorization":"Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI1ZWQzZGEzMDVkMDc4NjdjZjg4N2RhY2IiLCJpYXQiOjE1OTEwOTUxNjEsImV4cCI6MTU5MTI2Nzk2MX0.m4DLxbhchw3lpOQf8vY_1R985y9zPds_2kK1xnGVRxA"
  },
  url:"http://localhost:3000/v1/public/getlist",
 params:{
   category:'音乐'
 }
}).then(res=>{
  console.log(res.data)
})


```

## `POST`

```js
上传文件

let formdata = new FormData();
    formdata.append('file',event.target.files[0]);
    const res = await axios.post('https://imgkr.com/api/files/upload', data, {
        headers: {
          'Content-Type': 'multipart/form-data',
       }
      })
    
    
 export function createArticle(data) {
  return request({
    url: '/article/create',
    method: 'post',
    data
  })
}
```

## `拦截器`

```js
// 封装 axios
// 1.封装请求返回数据 2.异常统一处理
// 鉴权处理

import axios from 'axios'
import errorHandle from './errorHandle'

const instance = axios.create({
  // 统一请求配置
  baseURL:
    process.env.NODE_ENV === 'development'
      ? config.baseURL.dev
      : config.baseURL.pro,
  headers: {
    'Content-Type': 'application/json;charset=utf-8'
  },
  timeout: 10000
})


// 请求拦截器
instance.interceptors.request.use(
  config => {
    return config
  },
  // 请求异常处理
  err => {
    errorHandle(err)
    return Promise.reject(err)
  }
)

// 请求结果封装  
instance.interceptors.response.use(
  res => {
    if (res.status === 200) {
       // 直接返回res.data
      return Promise.resolve(res.data)
    } else {
      return Promise.reject(res)
    }
  },
  error => {
    // Any status codes that falls outside the range of 2xx cause this function to trigger
    // Do something with response error  处理非200的请求返回的异常: 比如404 ，API服务暂停(没有状态码)等
    errorHandle(error)
    return Promise.reject(error)
  }
)
```

```js
import {
  Message
} from 'element-ui'
const errorHandle = (error) => {
  const errorStatus = error.response.status
  switch (errorStatus) {
    case 401:
      console.log('刷新token')
      break
    case 500:
      Message({
        type: 'error',
        message: error.response.data.msg,
        duration: 4000
      })
      break
    case 404:
      Message({
        type: 'error',
        message: '网络异常',
        duration: 4000
      })
      break
    default:
      break
  }
}
```

