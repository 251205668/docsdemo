## 首页

> ! _base-url_ = 'https://shop.yangxiansheng.top/heyushuo'

> ! 都是GET请求

**获取首页数据**

**接口地址**
`GET /index/index`

**请求参数**

| 参数名称        | 是否必须           | 类型  | 说明  |
| ------------- |:-------------:| -----:| ----:|

**返回值**

| 参数名称                  | 类型  | 说明  |
| ------------- | ----:| ---:|
| banner(轮播)      | Array | 返回值 |
| channel(商品类别)      | Array | 返回值 |
| newGoods(新品上市)    | Array | 返回值 |
| hotGoods(热门商品)    | Array | 返回值 |
| brandList(品牌列表)    | Array | 返回值 |
| topicList(主题列表)    | Array | 返回值 |
| categoryList(所有的主类别)    | Array | 返回值 |
| newCategoryList (查询类别对应的子类别)    | Array | 返回值 |

**示例**

- 请求：[https://shop.yangxiansheng.top/heyushuo/index/index](https://shop.yangxiansheng.top/heyushuo/index/index)
- 响应：
  ![](https://image.yangxiansheng.top/img/QQ截图20200225230721.png?imagelist)

### 品牌制造商直供的列表

**接口地址**
`GET /brand/listaction`

**请求参数**

| 参数名称 | 是否必须 | 类型  | 说明  |
| ---- |:----:| ---:| ---:|

**返回值**

| 参数名称                  | 类型  | 说明  |
| ------------- | ----:| ---:|
| id   | Number | 返回值 |
| name     | String | 返回值 |
| floor_price    | Number | 返回值 |
| app_list_pic_url()  | String | 返回值 |

**示例**

- 请求：[https://shop.yangxiansheng.top/heyushuo/brand/listaction](https://shop.yangxiansheng.top/heyushuo/brand/listaction)
- 响应：
  ![](https://image.yangxiansheng.top/img/QQ截图20200225230721.png?imagelist)

### 品牌制造商直供的列表详情数据

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/brand/detailaction `

**请求方式：**

- GET 

**参数：** 

| 参数名 | 必选  | 类型  | 说明  |
|:--- |:--- |:--- | --- |
| id  | 是   | int | 无   |

**返回示例**

```json
{
  "data": {
    "id": 1001000,
    "name": "MUJI制造商",
    "list_pic_url": "http://yanxuan.nosdn.127.net/1541445967645114dd75f6b0edc4762d.png",
    "simple_desc": "严选精选了MUJI制造商和生产原料，\n用几乎零利润的价格，剔除品牌溢价，\n让用户享受原品牌的品质生活。",
    "pic_url": "http://yanxuan.nosdn.127.net/4ea3f1e60dd77c45c218e503d721a1ed.jpg",
    "sort_order": 2,
    "is_show": 1,
    "floor_price": 12.9,
    "app_list_pic_url": "http://yanxuan.nosdn.127.net/1541445967645114dd75f6b0edc4762d.png",
    "is_new": 1,
    "new_pic_url": "http://yanxuan.nosdn.127.net/4ea3f1e60dd77c45c218e503d721a1ed.jpg",
    "new_sort_order": 2
  },
  "goodsList": [
    {
      "id": 1009009,
      "category_id": 1008008,
      "goods_sn": "1009009",
      "name": "白鹅绒秋冬加厚羽绒被",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "热销5万条，一条被子过冬",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/79ae82326ba86985035215ca9bebd137.jpg\" _src=\"http://yanxuan.nosdn.127.net/79ae82326ba86985035215ca9bebd137.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7aadf2c5fd0942dc9bceb5a0738d969.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7aadf2c5fd0942dc9bceb5a0738d969.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ccf2486677aafef68048894317b6e96.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ccf2486677aafef68048894317b6e96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3ce70df9905a810c60220d9d24ebb2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3ce70df9905a810c60220d9d24ebb2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d51b1e4f61cb563b09dae46ee282e220.jpg\" _src=\"http://yanxuan.nosdn.127.net/d51b1e4f61cb563b09dae46ee282e220.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2791ef7173866f12be3341ca7202336.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2791ef7173866f12be3341ca7202336.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6cda9c3d9f044310f49afc5bbdb3533d.jpg\" _src=\"http://yanxuan.nosdn.127.net/6cda9c3d9f044310f49afc5bbdb3533d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/68e9be17108a9c6a0e6b786176a4b4c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/68e9be17108a9c6a0e6b786176a4b4c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3974579c71cdf946088d339e9e5c865d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3974579c71cdf946088d339e9e5c865d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d95a8520e3e3dfec063fc484e1d57207.jpg\" _src=\"http://yanxuan.nosdn.127.net/d95a8520e3e3dfec063fc484e1d57207.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce8b29a61396dced0f89ea3bfdf1f45d.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce8b29a61396dced0f89ea3bfdf1f45d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/129cba9ef941b367e56dad47aeb7fd96.jpg\" _src=\"http://yanxuan.nosdn.127.net/129cba9ef941b367e56dad47aeb7fd96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f566abb0c978093647aa1742725129ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/f566abb0c978093647aa1742725129ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7c7c153400895b5d690f1eba9b3c315.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7c7c153400895b5d690f1eba9b3c315.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be750a41eef4db163a29e2326a65660f.jpg\" _src=\"http://yanxuan.nosdn.127.net/be750a41eef4db163a29e2326a65660f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ea11ee2e846b3536acb599b93b7d2e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ea11ee2e846b3536acb599b93b7d2e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5814d4e02b3fd0b94d04ca262b201385.jpg\" _src=\"http://yanxuan.nosdn.127.net/5814d4e02b3fd0b94d04ca262b201385.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7959e1d91576bf0d21e7bd042e2210bd.jpg\" _src=\"http://yanxuan.nosdn.127.net/7959e1d91576bf0d21e7bd042e2210bd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4268cc5be26539ed427927e4e6d8e18e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4268cc5be26539ed427927e4e6d8e18e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5667dee42adfce79988974d96ddd8b09.jpg\" _src=\"http://yanxuan.nosdn.127.net/5667dee42adfce79988974d96ddd8b09.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6c9f0a1a51cd0166844d3694cc92a1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6c9f0a1a51cd0166844d3694cc92a1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce43457f50492c355ff1f7577685c004.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce43457f50492c355ff1f7577685c004.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c2ff68fede235b1b9f249cd5dabce0d.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c2ff68fede235b1b9f249cd5dabce0d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/785952cd32deedc2bfd90826e89ddc2a.jpg\" _src=\"http://yanxuan.nosdn.127.net/785952cd32deedc2bfd90826e89ddc2a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b544624dcc990b966e6c6d20ee608b7c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b544624dcc990b966e6c6d20ee608b7c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/761a606123be84d0c6eaa2e5eb9f4f81.jpg\" _src=\"http://yanxuan.nosdn.127.net/761a606123be84d0c6eaa2e5eb9f4f81.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0cce548176f68f7e00de503d4d146629.jpg\" _src=\"http://yanxuan.nosdn.127.net/0cce548176f68f7e00de503d4d146629.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/30cb73b7917af99d4ccbdbca9042d566.jpg\" _src=\"http://yanxuan.nosdn.127.net/30cb73b7917af99d4ccbdbca9042d566.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a27c57bb90e145df10d633dcfdbe26b.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a27c57bb90e145df10d633dcfdbe26b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8df76b01f83dd4d4a7f58014d8977067.jpg\" _src=\"http://yanxuan.nosdn.127.net/8df76b01f83dd4d4a7f58014d8977067.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ea47ed85b1334e2da9672ee3e9ad66a4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ea47ed85b1334e2da9672ee3e9ad66a4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/750caeba2fa63dec64d598e8299f2122.jpg\" _src=\"http://yanxuan.nosdn.127.net/750caeba2fa63dec64d598e8299f2122.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14bd429f1d48be5d9a8240c1fb4c494b.jpg\" _src=\"http://yanxuan.nosdn.127.net/14bd429f1d48be5d9a8240c1fb4c494b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02ee506d1f4ba045d7408a0b1e719c8e.jpg\" _src=\"http://yanxuan.nosdn.127.net/02ee506d1f4ba045d7408a0b1e719c8e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82443ff0a437048729b35fbdb85b0c3a.jpg\" _src=\"http://yanxuan.nosdn.127.net/82443ff0a437048729b35fbdb85b0c3a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3f39a87baa66fe50f3b141d148645b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3f39a87baa66fe50f3b141d148645b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/814e549460f206dccb8889165ef69ea2.jpg\" _src=\"http://yanxuan.nosdn.127.net/814e549460f206dccb8889165ef69ea2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/43c21522533725d57ff893f9d080f6cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/43c21522533725d57ff893f9d080f6cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfc0d18fa3b2ba721fd7614af7962cbe.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfc0d18fa3b2ba721fd7614af7962cbe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b58ac36c4781edd6d09dfeb2fbb6112.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b58ac36c4781edd6d09dfeb2fbb6112.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aadb34b1fe47217989e46eefb2fcef2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/aadb34b1fe47217989e46eefb2fcef2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/558aa961eb6b51692e50c5801d74adeb.jpg\" _src=\"http://yanxuan.nosdn.127.net/558aa961eb6b51692e50c5801d74adeb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af3a0c3d829d015c0850befa9aa7f05c.jpg\" _src=\"http://yanxuan.nosdn.127.net/af3a0c3d829d015c0850befa9aa7f05c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23c02d5a325df4c87eb339e694489339.jpg\" _src=\"http://yanxuan.nosdn.127.net/23c02d5a325df4c87eb339e694489339.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c51160264c2344feb8a2580d0c47a655.jpg\" _src=\"http://yanxuan.nosdn.127.net/c51160264c2344feb8a2580d0c47a655.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ea8ecd877fdd3c0b30f7d7b961fdf8ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/ea8ecd877fdd3c0b30f7d7b961fdf8ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5976f583518689c566c94ce65ac8fcb2.jpg\" _src=\"http://yanxuan.nosdn.127.net/5976f583518689c566c94ce65ac8fcb2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/494dc60b71027177448188093c5eb072.jpg\" _src=\"http://yanxuan.nosdn.127.net/494dc60b71027177448188093c5eb072.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c0fc3b0727795fe696579e6b3a1f817.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c0fc3b0727795fe696579e6b3a1f817.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ab7aa0de0e90b5a8768d25155e6c475.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ab7aa0de0e90b5a8768d25155e6c475.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/839ffe5bf65befd4ec353fbed7730b2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/839ffe5bf65befd4ec353fbed7730b2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/313df862cf6181ef199b782969be4607.jpg\" _src=\"http://yanxuan.nosdn.127.net/313df862cf6181ef199b782969be4607.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e39bfc4343d8968879ec66cc67db8987.jpg\" _src=\"http://yanxuan.nosdn.127.net/e39bfc4343d8968879ec66cc67db8987.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0c74814f38aba0c40a405ece465d554.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0c74814f38aba0c40a405ece465d554.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 19,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/47bb01a1c0d4940494d31e7a61e6466e.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/9791006f25e26b2d7c81f41f87ce8619.png",
      "retail_price": 1999,
      "sell_volume": 154,
      "primary_product_id": 1008012,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1011004,
      "category_id": 1036000,
      "goods_sn": "1011004",
      "name": "色织精梳AB纱格纹空调被",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "加大加厚，双色精彩",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/28680639193b939b5d93cd77b3272a1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/28680639193b939b5d93cd77b3272a1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/990c9a7781a8ae2b2a08c65c9af7afc7.jpg\" _src=\"http://yanxuan.nosdn.127.net/990c9a7781a8ae2b2a08c65c9af7afc7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7ccc07b50f491e94b6187bf49b48820.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7ccc07b50f491e94b6187bf49b48820.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69eb85fd08c9ebce511d13d899d96659.jpg\" _src=\"http://yanxuan.nosdn.127.net/69eb85fd08c9ebce511d13d899d96659.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a96f2f48217b913dc012671ed511d223.jpg\" _src=\"http://yanxuan.nosdn.127.net/a96f2f48217b913dc012671ed511d223.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c94a22b8644fafec3ff27f87dd12771b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c94a22b8644fafec3ff27f87dd12771b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/721b4749caada515bb5e616f41a410d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/721b4749caada515bb5e616f41a410d1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1215d6badb5a922efaeadd36911a4a3e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1215d6badb5a922efaeadd36911a4a3e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/749a3c6e9228d304806a06e478644ca1.jpg\" _src=\"http://yanxuan.nosdn.127.net/749a3c6e9228d304806a06e478644ca1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2cc7fd2eadbef5ab061fdf3550962d4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/2cc7fd2eadbef5ab061fdf3550962d4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/710b9318f02863fe79209e7e6c822a5a.jpg\" _src=\"http://yanxuan.nosdn.127.net/710b9318f02863fe79209e7e6c822a5a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaf8500212ec5bf783cb2bc63afbf7f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaf8500212ec5bf783cb2bc63afbf7f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f9e03dfb8cacda0f8fbbcf0ef20f8a62.jpg\" _src=\"http://yanxuan.nosdn.127.net/f9e03dfb8cacda0f8fbbcf0ef20f8a62.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3fa109d21bda840ac7040b196c13a871.jpg\" _src=\"http://yanxuan.nosdn.127.net/3fa109d21bda840ac7040b196c13a871.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76bfa90446c129fa3eb9f05104e9e778.jpg\" _src=\"http://yanxuan.nosdn.127.net/76bfa90446c129fa3eb9f05104e9e778.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3b94053478ceb6912a28597c51a3bcb.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3b94053478ceb6912a28597c51a3bcb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a25bca01f9ad835cd79b1c11ffdb400e.jpg\" _src=\"http://yanxuan.nosdn.127.net/a25bca01f9ad835cd79b1c11ffdb400e.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 2,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/4de19773ac86263bc5f474c1351c6df4.png",
      "list_pic_url": "http://yanxuan.nosdn.127.net/0984c9388a2c3fd2335779da904be393.png",
      "retail_price": 199,
      "sell_volume": 1007,
      "primary_product_id": 1010014,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 1
    },
    {
      "id": 1020000,
      "category_id": 1008002,
      "goods_sn": "1020000",
      "name": "升级款记忆绵护椎腰靠",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "人体工学设计，缓解腰背疼痛",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/8176934e414ec6c85078cb64322fe336.jpg\" _src=\"http://yanxuan.nosdn.127.net/8176934e414ec6c85078cb64322fe336.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33ff256b2f69de517f567ebb993dd08e.jpg\" _src=\"http://yanxuan.nosdn.127.net/33ff256b2f69de517f567ebb993dd08e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5204e4f7c7fa00866e270a93ec85a596.jpg\" _src=\"http://yanxuan.nosdn.127.net/5204e4f7c7fa00866e270a93ec85a596.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f3aed0164b92344f17ffbc0b8fc7ade.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f3aed0164b92344f17ffbc0b8fc7ade.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d2d94d8f0f10f17183954b69d09e2bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d2d94d8f0f10f17183954b69d09e2bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3921600dd00e2c49a7414035111b767d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3921600dd00e2c49a7414035111b767d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aef3c726fec0be6ce17089e06e753d4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/aef3c726fec0be6ce17089e06e753d4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/446fbad756b6327898cee40e7b67a0b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/446fbad756b6327898cee40e7b67a0b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0950b4fa1cac49eece29af35c6e69e4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/0950b4fa1cac49eece29af35c6e69e4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf7e88b2b57641ab81bbf36351db5ff8.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf7e88b2b57641ab81bbf36351db5ff8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d66b4714682aaff4ab082980a44b46.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d66b4714682aaff4ab082980a44b46.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7f2d82d7a5622dd9f6b0d44faed9fda.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7f2d82d7a5622dd9f6b0d44faed9fda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7fdc566d101b7cf73cee32f55b0f945.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7fdc566d101b7cf73cee32f55b0f945.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e04202364d1a0a1dc1a2a1ea871e45e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e04202364d1a0a1dc1a2a1ea871e45e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b3135ad6c01a2675fc7e96f6643ff7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b3135ad6c01a2675fc7e96f6643ff7f.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 15,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/84563d90b0c10c4d4a8229fd34cb4063.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/819fdf1f635a694166bcfdd426416e8c.png",
      "retail_price": 79,
      "sell_volume": 8586,
      "primary_product_id": 1018000,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1023012,
      "category_id": 1036000,
      "goods_sn": "1023012",
      "name": "色织华夫格夏凉被",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "凹凸华夫格织法，舒适轻柔",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/70e21fc5c723dc6adcb1b531553597d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/70e21fc5c723dc6adcb1b531553597d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fcdf78276ab0bcd8ed80a3dda8c29b6a.jpg\" _src=\"http://yanxuan.nosdn.127.net/fcdf78276ab0bcd8ed80a3dda8c29b6a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1eb088a53d00f094bbac4b1f7a662457.jpg\" _src=\"http://yanxuan.nosdn.127.net/1eb088a53d00f094bbac4b1f7a662457.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/86be51c377922edd23e48b9d0c51d5dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/86be51c377922edd23e48b9d0c51d5dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9cadf6589933fab072aef8c0644bb91.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9cadf6589933fab072aef8c0644bb91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/adbb912f1131f821f4d01bb29ed31450.jpg\" _src=\"http://yanxuan.nosdn.127.net/adbb912f1131f821f4d01bb29ed31450.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8309ca74e9ecea295882b68cc0080652.jpg\" _src=\"http://yanxuan.nosdn.127.net/8309ca74e9ecea295882b68cc0080652.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4cce90d2ad13258af815b828dd3fa34f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4cce90d2ad13258af815b828dd3fa34f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ad6cf5c7f4ed107d39997ce1acfffd2.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ad6cf5c7f4ed107d39997ce1acfffd2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b867cc1a9f3c0046b40118e009a2cbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b867cc1a9f3c0046b40118e009a2cbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b14b08ce203d77633340b1677f6196b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/b14b08ce203d77633340b1677f6196b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b697d210e3137bc9fa8f5b74a9916ce6.jpg\" _src=\"http://yanxuan.nosdn.127.net/b697d210e3137bc9fa8f5b74a9916ce6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8b23b600cb5848d00eb1a176554f5de.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8b23b600cb5848d00eb1a176554f5de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b76964151af30178e74e28d0d590fd7.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b76964151af30178e74e28d0d590fd7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3eda6586081f50314690ab9f141d1758.jpg\" _src=\"http://yanxuan.nosdn.127.net/3eda6586081f50314690ab9f141d1758.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/939f9ac497e48529e0c44ef5af32f329.jpg\" _src=\"http://yanxuan.nosdn.127.net/939f9ac497e48529e0c44ef5af32f329.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 4,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/8211ea549896095377d555b5066dbf82.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/07376e78bf4fb8a5aa8e6a0b1437c3ad.png",
      "retail_price": 299,
      "sell_volume": 7180,
      "primary_product_id": 1022030,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1023034,
      "category_id": 1036000,
      "goods_sn": "1023034",
      "name": "泡泡纱可水洗夏凉被",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "全棉泡泡纱，柔软亲肤",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/85eeb993c3b4f37680c1980ad142e076.jpg\" _src=\"http://yanxuan.nosdn.127.net/85eeb993c3b4f37680c1980ad142e076.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/81f6fb8e6d4917a25fd8b4817ea7d4f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/81f6fb8e6d4917a25fd8b4817ea7d4f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/accecd0efbee671b1592560c3e08df40.jpg\" _src=\"http://yanxuan.nosdn.127.net/accecd0efbee671b1592560c3e08df40.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1ed91aae1e7a9b3762edafcb31949b7.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1ed91aae1e7a9b3762edafcb31949b7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c08c0809a1ddfdc7f739666599920999.jpg\" _src=\"http://yanxuan.nosdn.127.net/c08c0809a1ddfdc7f739666599920999.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/233157394df91dc93fe61ab8d1103e79.jpg\" _src=\"http://yanxuan.nosdn.127.net/233157394df91dc93fe61ab8d1103e79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10f3d5dcab0458117539f5cf0929c268.jpg\" _src=\"http://yanxuan.nosdn.127.net/10f3d5dcab0458117539f5cf0929c268.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ce6ff785959f440508e3bc7a9348618.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ce6ff785959f440508e3bc7a9348618.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2b8c08729cfce7d9b35fd6ea00d4ba65.jpg\" _src=\"http://yanxuan.nosdn.127.net/2b8c08729cfce7d9b35fd6ea00d4ba65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d8284f1c706360ea32f8f05f94b367c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d8284f1c706360ea32f8f05f94b367c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e21927788dafa40a5f2f409114dca3c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/e21927788dafa40a5f2f409114dca3c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b3c8d2cc37f9fc533616a18cd7a655e.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b3c8d2cc37f9fc533616a18cd7a655e.jpg\" style=\"\"/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 5,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/55129640e1e09ff05e427c73d52a18c5.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/715899c65c023bb4973fb0466a5b79d6.png",
      "retail_price": 299,
      "sell_volume": 1068,
      "primary_product_id": 1031020,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1027004,
      "category_id": 1036000,
      "goods_sn": "1027004",
      "name": "色织六层纱布夏凉被",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "柔软纱布，婴童可用",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/67f90229027c9f7ce81be64b88a3a89d.jpg\" _src=\"http://yanxuan.nosdn.127.net/67f90229027c9f7ce81be64b88a3a89d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/938dcbd014d6651024b94ac9c61deeac.jpg\" _src=\"http://yanxuan.nosdn.127.net/938dcbd014d6651024b94ac9c61deeac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2afaf85ccfc966329c91873b9bcfd895.jpg\" _src=\"http://yanxuan.nosdn.127.net/2afaf85ccfc966329c91873b9bcfd895.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c7e46721c706d3a6abca8349384b7d29.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7e46721c706d3a6abca8349384b7d29.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16064cd765c185be8a4621ef66e3839e.jpg\" _src=\"http://yanxuan.nosdn.127.net/16064cd765c185be8a4621ef66e3839e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3861e21da16b8e8907136f167d011971.jpg\" _src=\"http://yanxuan.nosdn.127.net/3861e21da16b8e8907136f167d011971.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62035b349641dff662334c1f749930e3.jpg\" _src=\"http://yanxuan.nosdn.127.net/62035b349641dff662334c1f749930e3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d814f23d85fa7ba0d3871fbd2ca743c.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d814f23d85fa7ba0d3871fbd2ca743c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa41611ffce03535348c76548d7be717.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa41611ffce03535348c76548d7be717.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a88cf7d8a483148d5261ca6ea8888e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a88cf7d8a483148d5261ca6ea8888e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2ae01b731a6b50c78151f3fb270c2ee3.jpg\" _src=\"http://yanxuan.nosdn.127.net/2ae01b731a6b50c78151f3fb270c2ee3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/643974e12eea8a60e9b5c8039e2dfb46.jpg\" _src=\"http://yanxuan.nosdn.127.net/643974e12eea8a60e9b5c8039e2dfb46.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8866316ff84ac68d1fe347eb6db8b07.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8866316ff84ac68d1fe347eb6db8b07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8d875bd5949fa3d2f6bb1dbbcc12121.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8d875bd5949fa3d2f6bb1dbbcc12121.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3cc4a687ed3be8727ee90e371defb4d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/3cc4a687ed3be8727ee90e371defb4d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c519db001d883d017a133efc7080d41a.jpg\" _src=\"http://yanxuan.nosdn.127.net/c519db001d883d017a133efc7080d41a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbf012451cddac91a939c2b5171acc96.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbf012451cddac91a939c2b5171acc96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e63320cbbeecd593457e3ded8b5e9b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e63320cbbeecd593457e3ded8b5e9b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0acb487f97e14a5b9fc8c5fa5d8b1a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0acb487f97e14a5b9fc8c5fa5d8b1a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e4a709c0c8140be33d226e0963912499.jpg\" _src=\"http://yanxuan.nosdn.127.net/e4a709c0c8140be33d226e0963912499.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb3eaec97d07430ed6aea55e0a40b56e.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb3eaec97d07430ed6aea55e0a40b56e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/149f85abb95d094a7cb5ae7565a4ecd5.jpg\" _src=\"http://yanxuan.nosdn.127.net/149f85abb95d094a7cb5ae7565a4ecd5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af0c2642435d3437c9f710cc442615f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/af0c2642435d3437c9f710cc442615f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/592fd3838f55f48a3f4ba5b2e796eff2.jpg\" _src=\"http://yanxuan.nosdn.127.net/592fd3838f55f48a3f4ba5b2e796eff2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3433c1bb5f6e0e3f3a10481ec53a28f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/3433c1bb5f6e0e3f3a10481ec53a28f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/973cc6e90902c300a4648b5391246a19.jpg\" _src=\"http://yanxuan.nosdn.127.net/973cc6e90902c300a4648b5391246a19.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb348e33f7387db2ddeaac68ca1abde1.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb348e33f7387db2ddeaac68ca1abde1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7234ad4c588c7423cf121ffee298480.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7234ad4c588c7423cf121ffee298480.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/17f16b61bc645d686fdbed7be626bf4c.jpg\" _src=\"http://yanxuan.nosdn.127.net/17f16b61bc645d686fdbed7be626bf4c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6c3dc3c5436f3985a2fafce5e41d1e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6c3dc3c5436f3985a2fafce5e41d1e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d5adb3c164a8e9edb187ea20aaca8b41.jpg\" _src=\"http://yanxuan.nosdn.127.net/d5adb3c164a8e9edb187ea20aaca8b41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79e4f7477ee14c37ba3e8b34e51f70ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/79e4f7477ee14c37ba3e8b34e51f70ad.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 3,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a8dacc2f580c48bb535da34cf81c2497.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/6252f53aaf36c072b6678f3d8c635132.png",
      "retail_price": 249,
      "sell_volume": 1255,
      "primary_product_id": 1026004,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 1
    },
    {
      "id": 1039051,
      "category_id": 1008002,
      "goods_sn": "1039051",
      "name": "多功能午睡枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "放松自在的午后时光",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/aba5fac220a511eb859ad4834fd7c0e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/aba5fac220a511eb859ad4834fd7c0e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37c7411fe03ac22b8b924190a5c6f483.jpg\" _src=\"http://yanxuan.nosdn.127.net/37c7411fe03ac22b8b924190a5c6f483.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88e313d81b848936d673edebc823f617.jpg\" _src=\"http://yanxuan.nosdn.127.net/88e313d81b848936d673edebc823f617.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/efddbb9e7105a72fb40f168813764297.jpg\" _src=\"http://yanxuan.nosdn.127.net/efddbb9e7105a72fb40f168813764297.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4830e1927e472f45940a92acf3e04331.jpg\" _src=\"http://yanxuan.nosdn.127.net/4830e1927e472f45940a92acf3e04331.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10b2f2989c7239bcea42be91d1826fc7.jpg\" _src=\"http://yanxuan.nosdn.127.net/10b2f2989c7239bcea42be91d1826fc7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3d19a5320eb179b3752458f15f1a068.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3d19a5320eb179b3752458f15f1a068.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97a9d81d01cbc6c8bf57e8b308de1537.jpg\" _src=\"http://yanxuan.nosdn.127.net/97a9d81d01cbc6c8bf57e8b308de1537.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/500497dcf877fbf29548ef7eae7766fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/500497dcf877fbf29548ef7eae7766fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92f6105f284bdd94aa4b6495a7d43994.jpg\" _src=\"http://yanxuan.nosdn.127.net/92f6105f284bdd94aa4b6495a7d43994.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60161ebc38b0b8c8ca9de8a0165843bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/60161ebc38b0b8c8ca9de8a0165843bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ce9817e2d4415c5789028c57c593450.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ce9817e2d4415c5789028c57c593450.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e3dc4f7c9dcd228a94cc4ffa6cea1be.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e3dc4f7c9dcd228a94cc4ffa6cea1be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89360198abf4bbb4c108bfe1068d83b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/89360198abf4bbb4c108bfe1068d83b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f40b5ba3618e61e80ad8f175b3da866.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f40b5ba3618e61e80ad8f175b3da866.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad590b8d9cb20c046d0d8e68ea3b0dc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad590b8d9cb20c046d0d8e68ea3b0dc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c606522a6032f1a2268a0ee0d8d01dff.jpg\" _src=\"http://yanxuan.nosdn.127.net/c606522a6032f1a2268a0ee0d8d01dff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f226b9e158f2cf451e925a606d1b5ecd.jpg\" _src=\"http://yanxuan.nosdn.127.net/f226b9e158f2cf451e925a606d1b5ecd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b169357e50d02d557c468588939c7f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b169357e50d02d557c468588939c7f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5e676b79ffc838a2c496134c8c3f55f.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5e676b79ffc838a2c496134c8c3f55f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e934b380901ffa4b035825b82246634e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e934b380901ffa4b035825b82246634e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8decfed210a7ada28bd71496a8ef51a.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8decfed210a7ada28bd71496a8ef51a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fcc94c2ee6ea13ef7cd7d21f1c63b79.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fcc94c2ee6ea13ef7cd7d21f1c63b79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8bae5453415f2fd519b5cf836e9baddc.jpg\" _src=\"http://yanxuan.nosdn.127.net/8bae5453415f2fd519b5cf836e9baddc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5833f7b80c040d8bdf23e514d430e045.jpg\" _src=\"http://yanxuan.nosdn.127.net/5833f7b80c040d8bdf23e514d430e045.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15df0095ff692e8d67185c93c44680c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/15df0095ff692e8d67185c93c44680c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32fdd19de26dee3281e76dc33059b1f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/32fdd19de26dee3281e76dc33059b1f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/290d679b2fe2154ef36b777525d988bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/290d679b2fe2154ef36b777525d988bc.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99233a211060d951818a729d43bb6533.jpg\" _src=\"http://yanxuan.nosdn.127.net/99233a211060d951818a729d43bb6533.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76fcb532c1aa2f631c0e439f5986654f.jpg\" _src=\"http://yanxuan.nosdn.127.net/76fcb532c1aa2f631c0e439f5986654f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2e90d2089e907d605e1eee0e6fcb1d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2e90d2089e907d605e1eee0e6fcb1d1.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 14,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/20e7e05935a347b36adac369efc490c3.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/c8ca0600fa7ba11ca8be6a3173dd38c9.png",
      "retail_price": 79,
      "sell_volume": 8202,
      "primary_product_id": 1038068,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1043005,
      "category_id": 1008002,
      "goods_sn": "1043005",
      "name": "日式记忆绵坐垫",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "活性炭记忆绵，缓解压力",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/7239e35762ea2937549f53f4482124fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/7239e35762ea2937549f53f4482124fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c23c022ad6737aa351140d7ce97a4a43.jpg\" _src=\"http://yanxuan.nosdn.127.net/c23c022ad6737aa351140d7ce97a4a43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b6fe3f499101077e6ee595a9145172c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b6fe3f499101077e6ee595a9145172c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fdc843045b99838abd8ce3fcbec2890.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fdc843045b99838abd8ce3fcbec2890.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14d3e1c384f5bc66e85b4dfff61f49ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/14d3e1c384f5bc66e85b4dfff61f49ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14eed3d4524fe441a54b604f37cfd299.jpg\" _src=\"http://yanxuan.nosdn.127.net/14eed3d4524fe441a54b604f37cfd299.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1b3a30c34e6fecf8105bf430e6d547f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1b3a30c34e6fecf8105bf430e6d547f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb5411b150ce5a69c0f88ef3af918061.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb5411b150ce5a69c0f88ef3af918061.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aebe8243acfa28a42d300d985c6e7036.jpg\" _src=\"http://yanxuan.nosdn.127.net/aebe8243acfa28a42d300d985c6e7036.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1371f124f86fc38c195f49e4bf26ddc5.jpg\" _src=\"http://yanxuan.nosdn.127.net/1371f124f86fc38c195f49e4bf26ddc5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd05471ebf5529464c85eace3e7c5c7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd05471ebf5529464c85eace3e7c5c7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c607e963758e4ad3f3bc749098fdcec.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c607e963758e4ad3f3bc749098fdcec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd472e779f1748937d269b87464722b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd472e779f1748937d269b87464722b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d19ec3e68922cdae4da8c0ab174bf5eb.jpg\" _src=\"http://yanxuan.nosdn.127.net/d19ec3e68922cdae4da8c0ab174bf5eb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44003fe38ab817003cb441ed5e518c41.jpg\" _src=\"http://yanxuan.nosdn.127.net/44003fe38ab817003cb441ed5e518c41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f3a7c45c70930950e60ddac979953d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f3a7c45c70930950e60ddac979953d5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77fc74a83c328dddf610a045277f094e.jpg\" _src=\"http://yanxuan.nosdn.127.net/77fc74a83c328dddf610a045277f094e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14056056c8e8cf3f77a479de696d18ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/14056056c8e8cf3f77a479de696d18ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ec2764b8b29c67af332cc1fde825b70.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ec2764b8b29c67af332cc1fde825b70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/494504fdb2d59d924de16cf79629dee9.jpg\" _src=\"http://yanxuan.nosdn.127.net/494504fdb2d59d924de16cf79629dee9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddf59afdada25b6b7aad72aaf8f0af20.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddf59afdada25b6b7aad72aaf8f0af20.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b8ad80c319aac920f3409bcd4376e17.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b8ad80c319aac920f3409bcd4376e17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8571525a4f280d09926a1b388d06fe8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/8571525a4f280d09926a1b388d06fe8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23c8bb2834f9ec05adb69e4df8354224.jpg\" _src=\"http://yanxuan.nosdn.127.net/23c8bb2834f9ec05adb69e4df8354224.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9c44aea67b0392547fdb3ba7f24c5fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9c44aea67b0392547fdb3ba7f24c5fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5045464902396b85ea12724ed962d7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5045464902396b85ea12724ed962d7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f484b21d07738839d1e199d8ba1031f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/f484b21d07738839d1e199d8ba1031f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21718c637256576c66876aa30653e29d.jpg\" _src=\"http://yanxuan.nosdn.127.net/21718c637256576c66876aa30653e29d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 11,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/aedfe3b7d76361d104a425ff551ade77.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/2a95b16f5b147cab4845641bee738a2e.png",
      "retail_price": 59,
      "sell_volume": 7482,
      "primary_product_id": 1041015,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1048005,
      "category_id": 1008002,
      "goods_sn": "1048005",
      "name": "日式色织水洗条纹抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "色织面料，水洗工艺，柔软亲肤",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/39afc6f165cf752e16c199b65ab61ee8.jpg\" _src=\"http://yanxuan.nosdn.127.net/39afc6f165cf752e16c199b65ab61ee8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2635f2eb08e98687a132a97642d87de.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2635f2eb08e98687a132a97642d87de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08b6bca750a85d833740e1f12e5a6216.jpg\" _src=\"http://yanxuan.nosdn.127.net/08b6bca750a85d833740e1f12e5a6216.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f61f9587dc8aec8330335da87dbb60ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/f61f9587dc8aec8330335da87dbb60ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f22282ebbbeb664ba706e4f088c9db2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/f22282ebbbeb664ba706e4f088c9db2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad7819c5597db9fce742cbc61aa53c72.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad7819c5597db9fce742cbc61aa53c72.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ee4a43824784e660f44e16274c4717ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/ee4a43824784e660f44e16274c4717ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f0eb752fd857fa1af74602afadabb0fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/f0eb752fd857fa1af74602afadabb0fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/46290c0b824babab46ce73feb23a554d.jpg\" _src=\"http://yanxuan.nosdn.127.net/46290c0b824babab46ce73feb23a554d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1c34134e19df505b4b1b2277880bba2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1c34134e19df505b4b1b2277880bba2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0bce553f09f5146ba9209264c46e38ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/0bce553f09f5146ba9209264c46e38ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/732ed69a0539f4d972213ed64e5bcff0.jpg\" _src=\"http://yanxuan.nosdn.127.net/732ed69a0539f4d972213ed64e5bcff0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/147fcd503618a36a76ed792c6a2254b1.jpg\" _src=\"http://yanxuan.nosdn.127.net/147fcd503618a36a76ed792c6a2254b1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f68cea7d1e7dd23349f7c36e366cb6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f68cea7d1e7dd23349f7c36e366cb6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/852711207b87360d29289be16a76e5ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/852711207b87360d29289be16a76e5ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f46c1d0edb91be4fa7c2747b423c494.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f46c1d0edb91be4fa7c2747b423c494.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f2bc29d55899694b917c9991d0b1333.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f2bc29d55899694b917c9991d0b1333.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63d4fa2caa8bbd1d7e205e90fe176633.jpg\" _src=\"http://yanxuan.nosdn.127.net/63d4fa2caa8bbd1d7e205e90fe176633.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f885db84f7911c3c4abc9695f55f19f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/f885db84f7911c3c4abc9695f55f19f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd0c5be6c986a60a577ab7fd4fa9796e.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd0c5be6c986a60a577ab7fd4fa9796e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb0f814679347c4876f2ca30acd57f88.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb0f814679347c4876f2ca30acd57f88.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/64b5936ea7e076885a7c1611d492aa57.jpg\" _src=\"http://yanxuan.nosdn.127.net/64b5936ea7e076885a7c1611d492aa57.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b503dd5b259a049dc3fffcabe6264c10.jpg\" _src=\"http://yanxuan.nosdn.127.net/b503dd5b259a049dc3fffcabe6264c10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3fb47a70640f6c252518a80a803bd362.jpg\" _src=\"http://yanxuan.nosdn.127.net/3fb47a70640f6c252518a80a803bd362.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1837c9a132b1ca0ed52f76f935563b7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1837c9a132b1ca0ed52f76f935563b7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09e9cc037e909c934aba0b87c48914ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/09e9cc037e909c934aba0b87c48914ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5c3a85ee4217386a8161016aa7727b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5c3a85ee4217386a8161016aa7727b9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e666622ecebc8fc733a49c5ad7d16c3e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e666622ecebc8fc733a49c5ad7d16c3e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48f87049ad7e2492ae75da78b97cd6fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/48f87049ad7e2492ae75da78b97cd6fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21cc4790d10496f2e73531c420fbb394.jpg\" _src=\"http://yanxuan.nosdn.127.net/21cc4790d10496f2e73531c420fbb394.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9510a74920b5589cba7af910774f8c0c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9510a74920b5589cba7af910774f8c0c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c69b713c98187890316668d10aa55c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c69b713c98187890316668d10aa55c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dcafde6d38fd075c4ba6d0cc1e816314.jpg\" _src=\"http://yanxuan.nosdn.127.net/dcafde6d38fd075c4ba6d0cc1e816314.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ccdf51824645c27ab06e78faa85db7d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ccdf51824645c27ab06e78faa85db7d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8096a502cac9f926d288cbbe8b8534fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/8096a502cac9f926d288cbbe8b8534fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b2b9a1f8a1422e3975cbee85685672c.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b2b9a1f8a1422e3975cbee85685672c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fd6779619cc7ed6f2a4057526f0c579d.jpg\" _src=\"http://yanxuan.nosdn.127.net/fd6779619cc7ed6f2a4057526f0c579d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdef4d1620407043511daf2e97746f07.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdef4d1620407043511daf2e97746f07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f30d798c772ea1599723c427c1d643b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f30d798c772ea1599723c427c1d643b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0cfc9aae9304010e24d92b29220dc0b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/0cfc9aae9304010e24d92b29220dc0b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e20e47f1eaf643bc569ccb148781529.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e20e47f1eaf643bc569ccb148781529.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9beb4226eb47be1c16e872dd9281634.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9beb4226eb47be1c16e872dd9281634.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70d2d737fbf7fc5980604ea294942b41.jpg\" _src=\"http://yanxuan.nosdn.127.net/70d2d737fbf7fc5980604ea294942b41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/496224b05a3054625b065de6aa769959.jpg\" _src=\"http://yanxuan.nosdn.127.net/496224b05a3054625b065de6aa769959.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0671941e0dfb696d5392f174a949a13.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0671941e0dfb696d5392f174a949a13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2df72e131e86e433d939776783a44db7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2df72e131e86e433d939776783a44db7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3bea99ca3040befe69d4811e0ef9b226.jpg\" _src=\"http://yanxuan.nosdn.127.net/3bea99ca3040befe69d4811e0ef9b226.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbc003f18889ab46a5a3a7e8698df351.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbc003f18889ab46a5a3a7e8698df351.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ee0df8d583844e734273d73eb582a4a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ee0df8d583844e734273d73eb582a4a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ea9467e6f4ef5c8f0812c1595704840.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ea9467e6f4ef5c8f0812c1595704840.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 5,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2167445c1b3df028d660bb992f321396.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ce980c16810a471dffff6aa8d7bac754.png",
      "retail_price": 59,
      "sell_volume": 5846,
      "primary_product_id": 1047014,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1055016,
      "category_id": 1008002,
      "goods_sn": "1055016",
      "name": "日式纯棉针织条纹抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "亲肤舒适，宛如妈妈的怀抱",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/4060bcde249c2501e5d95cfa0888a6c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/4060bcde249c2501e5d95cfa0888a6c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afebd965217cfdbc238de9252c7d6e37.jpg\" _src=\"http://yanxuan.nosdn.127.net/afebd965217cfdbc238de9252c7d6e37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b017649229c04dad59c312b3fe0cf7be.jpg\" _src=\"http://yanxuan.nosdn.127.net/b017649229c04dad59c312b3fe0cf7be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e02d923a92d5bef4b264381cffd5d813.jpg\" _src=\"http://yanxuan.nosdn.127.net/e02d923a92d5bef4b264381cffd5d813.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0447366651e06dde345c907e12315c73.jpg\" _src=\"http://yanxuan.nosdn.127.net/0447366651e06dde345c907e12315c73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5fdb8a54a2bc2285d1136bf9a2a674f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5fdb8a54a2bc2285d1136bf9a2a674f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1836dd3b75444a3ce42dc49fa5ee513.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1836dd3b75444a3ce42dc49fa5ee513.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f4740ae47c3ca8465e1ea6ec0a43563.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f4740ae47c3ca8465e1ea6ec0a43563.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f9f33a85933788209e6195468044387.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f9f33a85933788209e6195468044387.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b6ceab4330e0dd218db3c16582465be1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b6ceab4330e0dd218db3c16582465be1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dea7df197ba1e5ce5e9646aea43f798.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dea7df197ba1e5ce5e9646aea43f798.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/022e305413c9aa8e8db30a46a2a65286.jpg\" _src=\"http://yanxuan.nosdn.127.net/022e305413c9aa8e8db30a46a2a65286.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cce2571a59a0bc39784d61c4134f9458.jpg\" _src=\"http://yanxuan.nosdn.127.net/cce2571a59a0bc39784d61c4134f9458.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1f287dab80d1b11450051de6c119611.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1f287dab80d1b11450051de6c119611.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7b6318cb7623349542ba971cf1887da.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7b6318cb7623349542ba971cf1887da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf56a8ae91e07c91d70cf7b88cb59676.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf56a8ae91e07c91d70cf7b88cb59676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76aebdbc4a150837b2dcaa2293c85cc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/76aebdbc4a150837b2dcaa2293c85cc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/902fb302066a65488ed1f6da3a16ed66.jpg\" _src=\"http://yanxuan.nosdn.127.net/902fb302066a65488ed1f6da3a16ed66.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd9df2852e760940b0ab9e599320ed35.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd9df2852e760940b0ab9e599320ed35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ad1c6c9e619df09685cf9596339d714.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ad1c6c9e619df09685cf9596339d714.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83e54a3b9d13dc3c67e880c02e63167c.jpg\" _src=\"http://yanxuan.nosdn.127.net/83e54a3b9d13dc3c67e880c02e63167c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f6b75fe4ff9ae0b976c8c85bbf0a719.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f6b75fe4ff9ae0b976c8c85bbf0a719.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82f850ea52ca3e7048283b3f8a65c616.jpg\" _src=\"http://yanxuan.nosdn.127.net/82f850ea52ca3e7048283b3f8a65c616.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5bd4faa4898d9ea3c56fba9c5749cc62.jpg\" _src=\"http://yanxuan.nosdn.127.net/5bd4faa4898d9ea3c56fba9c5749cc62.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6488dedf51c6e5a90fc5f156a4e8416b.jpg\" _src=\"http://yanxuan.nosdn.127.net/6488dedf51c6e5a90fc5f156a4e8416b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bc667ddb5116ceaf329f55982da36bb1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bc667ddb5116ceaf329f55982da36bb1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfbfde943773a0258fa81b84d710d36e.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfbfde943773a0258fa81b84d710d36e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60d64bb0ac51346dc39d266beacdb846.jpg\" _src=\"http://yanxuan.nosdn.127.net/60d64bb0ac51346dc39d266beacdb846.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c50c0fd364d6b9a8646d0da75ce48f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c50c0fd364d6b9a8646d0da75ce48f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b24da9df819efdf9e110bb2228eadf0d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b24da9df819efdf9e110bb2228eadf0d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3cbbd9ec8dd41be2b35bf49842b67d86.jpg\" _src=\"http://yanxuan.nosdn.127.net/3cbbd9ec8dd41be2b35bf49842b67d86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d5bb53b92ed48f3f81980e41b51c0fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d5bb53b92ed48f3f81980e41b51c0fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d75a8fd77357f9a74a36fd7bfa7cebed.jpg\" _src=\"http://yanxuan.nosdn.127.net/d75a8fd77357f9a74a36fd7bfa7cebed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2dd8069e6739d732a53c25c74c0b2a89.jpg\" _src=\"http://yanxuan.nosdn.127.net/2dd8069e6739d732a53c25c74c0b2a89.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d7b4e172f8fd168e28854c3d8d04c56f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d7b4e172f8fd168e28854c3d8d04c56f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8b981b58ffb3e0a75916def11e45493.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8b981b58ffb3e0a75916def11e45493.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fb12dd3d12c8828a5cf2e16f17a8f27.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fb12dd3d12c8828a5cf2e16f17a8f27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8df57201eb9f5e7b576a6ccc31286e8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8df57201eb9f5e7b576a6ccc31286e8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f86f20ab83206abfdd682418e3cd3ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f86f20ab83206abfdd682418e3cd3ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c64ea783c9bd6dd2cb51b9978769edb.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c64ea783c9bd6dd2cb51b9978769edb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/104dca8bdfb6413fed5379a5b04eec10.jpg\" _src=\"http://yanxuan.nosdn.127.net/104dca8bdfb6413fed5379a5b04eec10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2cfb7760b81f0a82bdbae5079bfcd5ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/2cfb7760b81f0a82bdbae5079bfcd5ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1c6e09984c0599b5205f4d099cd5cfcb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1c6e09984c0599b5205f4d099cd5cfcb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e32f3a0bbc7ba3ec49b69fa89ba7da39.jpg\" _src=\"http://yanxuan.nosdn.127.net/e32f3a0bbc7ba3ec49b69fa89ba7da39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/408bf6b2815efea1020278ff57204667.jpg\" _src=\"http://yanxuan.nosdn.127.net/408bf6b2815efea1020278ff57204667.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6707b10b7a14f7d2e7487f30a687cfb2.jpg\" _src=\"http://yanxuan.nosdn.127.net/6707b10b7a14f7d2e7487f30a687cfb2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c4977d2ce8691f85575698990c13c3a.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c4977d2ce8691f85575698990c13c3a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22213164e3ce12c23260519cc5f2dd7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/22213164e3ce12c23260519cc5f2dd7f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9c8f7fda81f79cec8e75404386677c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9c8f7fda81f79cec8e75404386677c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1e5093b54f817ed1906fc58e7494790.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1e5093b54f817ed1906fc58e7494790.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/162452d2cb5ad3348862d5b1da7348c5.jpg\" _src=\"http://yanxuan.nosdn.127.net/162452d2cb5ad3348862d5b1da7348c5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8f6de9bc947bed7d5cebfe1f49a786d.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8f6de9bc947bed7d5cebfe1f49a786d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 8,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/8132003a8940c7056960c3c5fce59903.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/23e0203f1512f33e605f61c28fa03d2d.png",
      "retail_price": 59,
      "sell_volume": 948,
      "primary_product_id": 1056032,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1057036,
      "category_id": 1008002,
      "goods_sn": "1057036",
      "name": "日式纯色水洗亚麻抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "水洗亚麻，透气亲肤",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/6b69f7597ccffd27d77467d9d04eb294.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b69f7597ccffd27d77467d9d04eb294.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a89ca371ef07355c1feb293db961bd30.jpg\" _src=\"http://yanxuan.nosdn.127.net/a89ca371ef07355c1feb293db961bd30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2076e89c5f8fde4f44f918bd02d18eb7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2076e89c5f8fde4f44f918bd02d18eb7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5c9111e4dcc13cb41db98f68086cc620.jpg\" _src=\"http://yanxuan.nosdn.127.net/5c9111e4dcc13cb41db98f68086cc620.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f0645abcf883e7a863f32ce95f3c26b.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f0645abcf883e7a863f32ce95f3c26b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76a2b12f2d0f48f268d18b0ca0d1d6bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/76a2b12f2d0f48f268d18b0ca0d1d6bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a91f75159867f33a91f4e9992e00afa1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a91f75159867f33a91f4e9992e00afa1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93de61256a8ff3a8aa4bb90847ff454e.jpg\" _src=\"http://yanxuan.nosdn.127.net/93de61256a8ff3a8aa4bb90847ff454e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f611f99bea2920881e1421c110970234.jpg\" _src=\"http://yanxuan.nosdn.127.net/f611f99bea2920881e1421c110970234.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a292339423f141ad5d7a4011ea316956.jpg\" _src=\"http://yanxuan.nosdn.127.net/a292339423f141ad5d7a4011ea316956.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2045ae4f861d9eae6af351b9d82c9239.jpg\" _src=\"http://yanxuan.nosdn.127.net/2045ae4f861d9eae6af351b9d82c9239.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/398718a6d579c4af5f255909283e44a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/398718a6d579c4af5f255909283e44a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5be95e2db627908d23605fe042af2937.jpg\" _src=\"http://yanxuan.nosdn.127.net/5be95e2db627908d23605fe042af2937.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50a4fa0f67aa85dfaad36695225fe2f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/50a4fa0f67aa85dfaad36695225fe2f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c825e297cfbaaae632146a55c61dc3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c825e297cfbaaae632146a55c61dc3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/261c7819e7e9ac165e64cae88a59f70c.jpg\" _src=\"http://yanxuan.nosdn.127.net/261c7819e7e9ac165e64cae88a59f70c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec83f40d91fcc79f59a2479dffeb4565.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec83f40d91fcc79f59a2479dffeb4565.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/26f3e85402086b7d261a650e244dc676.jpg\" _src=\"http://yanxuan.nosdn.127.net/26f3e85402086b7d261a650e244dc676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dccb68f0d97112d245ab1924744b94b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/dccb68f0d97112d245ab1924744b94b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaba69949efd7ed85e72071f4ade4945.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaba69949efd7ed85e72071f4ade4945.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f23300061e5cf871e86a51f0012e885.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f23300061e5cf871e86a51f0012e885.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a55eedca057e0c973549ac8f13b47800.jpg\" _src=\"http://yanxuan.nosdn.127.net/a55eedca057e0c973549ac8f13b47800.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abf16e831285e3d97dbb60a3162e7968.jpg\" _src=\"http://yanxuan.nosdn.127.net/abf16e831285e3d97dbb60a3162e7968.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9390c8dab9fc7d8c27ac9410eb0340c.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9390c8dab9fc7d8c27ac9410eb0340c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8feb2be5afec5abe439cf1b42683373f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8feb2be5afec5abe439cf1b42683373f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/beb7620d0f685ab9c3af7ed18284b29e.jpg\" _src=\"http://yanxuan.nosdn.127.net/beb7620d0f685ab9c3af7ed18284b29e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f70ceed2078d44d747a9ce369feee9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f70ceed2078d44d747a9ce369feee9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5469e219bd5347568337746b257f094e.jpg\" _src=\"http://yanxuan.nosdn.127.net/5469e219bd5347568337746b257f094e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a177a6b6e58580809330895ebdbaff6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/a177a6b6e58580809330895ebdbaff6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9db0090d56ab757babb2ba661726cbe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/9db0090d56ab757babb2ba661726cbe3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6363637e0dd2fc670745c217b2a5cbfc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6363637e0dd2fc670745c217b2a5cbfc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1af1bde98f1497f591f62bff99ccca54.jpg\" _src=\"http://yanxuan.nosdn.127.net/1af1bde98f1497f591f62bff99ccca54.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69d034b353ae2e6e30afb6c21483690f.jpg\" _src=\"http://yanxuan.nosdn.127.net/69d034b353ae2e6e30afb6c21483690f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e29d6ac5ed040d63847ca456a179d43.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e29d6ac5ed040d63847ca456a179d43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29e460fba57f67cd83121f6cb917cfbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/29e460fba57f67cd83121f6cb917cfbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16090c02f4d4b76c6be82d98e489586e.jpg\" _src=\"http://yanxuan.nosdn.127.net/16090c02f4d4b76c6be82d98e489586e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c840eb66cf002227c52a13fbe55f657b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c840eb66cf002227c52a13fbe55f657b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16f65265b0942a60f3241704dc29be13.jpg\" _src=\"http://yanxuan.nosdn.127.net/16f65265b0942a60f3241704dc29be13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54a63da54b4e80867d8cd92d1ea9576e.jpg\" _src=\"http://yanxuan.nosdn.127.net/54a63da54b4e80867d8cd92d1ea9576e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebd0b906076850983e5a2aae9f667ce7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebd0b906076850983e5a2aae9f667ce7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bbf32cdc82643a85c12ff05ea88088ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/bbf32cdc82643a85c12ff05ea88088ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca6e3ccc3725c3f58338b62a5a0655d3.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca6e3ccc3725c3f58338b62a5a0655d3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ef02962e6155f811566aad168dabbec.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ef02962e6155f811566aad168dabbec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/832735166071f05288ffd347dff58ee6.jpg\" _src=\"http://yanxuan.nosdn.127.net/832735166071f05288ffd347dff58ee6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4fc490c4e9a0a0fa0affd317b8526f4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4fc490c4e9a0a0fa0affd317b8526f4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b05f975f16c09f106c81533c1a249b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b05f975f16c09f106c81533c1a249b0.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 6,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/f40fffd36cc85d5e0cf69417f4192ac1.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/8a9ee5ba08929cc9e40b973607d2f633.png",
      "retail_price": 79,
      "sell_volume": 1727,
      "primary_product_id": 1058097,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1075024,
      "category_id": 1008008,
      "goods_sn": "1075024",
      "name": "升级款纯棉静音白鹅羽绒被",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "静音面料，加厚熟睡",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/56261ca3bfb33b4400911bd01ac27ae5.jpg\" _src=\"http://yanxuan.nosdn.127.net/56261ca3bfb33b4400911bd01ac27ae5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/214f8c19371d71dac57ec63e398e87bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/214f8c19371d71dac57ec63e398e87bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/12732b11ddc970e10ebf37d71088bab3.jpg\" _src=\"http://yanxuan.nosdn.127.net/12732b11ddc970e10ebf37d71088bab3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be6a7afdc814c8f56d08e3f4285cd456.jpg\" _src=\"http://yanxuan.nosdn.127.net/be6a7afdc814c8f56d08e3f4285cd456.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/67cca9bceb817b16690e291a67f41e28.jpg\" _src=\"http://yanxuan.nosdn.127.net/67cca9bceb817b16690e291a67f41e28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/67313c9944f3e4277c3e640ab60bbde3.jpg\" _src=\"http://yanxuan.nosdn.127.net/67313c9944f3e4277c3e640ab60bbde3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/47235be353e7eec56b7e425be4ddedba.jpg\" _src=\"http://yanxuan.nosdn.127.net/47235be353e7eec56b7e425be4ddedba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3e3d7887ec3ea8ddabd581c4e36e2f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3e3d7887ec3ea8ddabd581c4e36e2f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33f1565e2a14c3fb4456b694771e6fad.jpg\" _src=\"http://yanxuan.nosdn.127.net/33f1565e2a14c3fb4456b694771e6fad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7a41d8674cd63d15c5549a6c5745a658.jpg\" _src=\"http://yanxuan.nosdn.127.net/7a41d8674cd63d15c5549a6c5745a658.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7522e4b7add69ae6ba223a38fbd34f4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/7522e4b7add69ae6ba223a38fbd34f4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5c9bd7dae7c24125104e80384c602ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5c9bd7dae7c24125104e80384c602ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97a225e49a0a8c764ca394cccb3b10f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/97a225e49a0a8c764ca394cccb3b10f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16f06738c9fb6355352a4eb21a25744b.jpg\" _src=\"http://yanxuan.nosdn.127.net/16f06738c9fb6355352a4eb21a25744b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3ad7de130695e388afa4946c63b4214.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3ad7de130695e388afa4946c63b4214.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0dd0e528b444841f7326dc933b501938.jpg\" _src=\"http://yanxuan.nosdn.127.net/0dd0e528b444841f7326dc933b501938.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ae9599dba84e72c970eecafd9de6294.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ae9599dba84e72c970eecafd9de6294.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b93b7087d8c64647b725418211fd2c4b.jpg\" _src=\"http://yanxuan.nosdn.127.net/b93b7087d8c64647b725418211fd2c4b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ff7f4cae6011903f209305cd57598c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ff7f4cae6011903f209305cd57598c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/123723b1a400f6088af024190f154d01.jpg\" _src=\"http://yanxuan.nosdn.127.net/123723b1a400f6088af024190f154d01.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3a6127948261397e2cce816afe7ff10.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3a6127948261397e2cce816afe7ff10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2bc185f49542115c38aca6508951f83.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2bc185f49542115c38aca6508951f83.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf2a0932d6fd65702b0d30dee3f1c658.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf2a0932d6fd65702b0d30dee3f1c658.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f02e979aff1ce7a335cd314491886b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f02e979aff1ce7a335cd314491886b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1c64f22b8da97967e854b6e2240ba8ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/1c64f22b8da97967e854b6e2240ba8ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/857365c29c631ca06d9218213e54f3d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/857365c29c631ca06d9218213e54f3d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be2f36d6255a9f8baf5573c8cb80b4c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/be2f36d6255a9f8baf5573c8cb80b4c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e1f71db51b1e322046737356482f115e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e1f71db51b1e322046737356482f115e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0697d1c2cd446297ad0494fc97f75ebb.jpg\" _src=\"http://yanxuan.nosdn.127.net/0697d1c2cd446297ad0494fc97f75ebb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e663a704ca44c6d448d37a9fbfb34b1.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e663a704ca44c6d448d37a9fbfb34b1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5cc03a916aa7a1a7160aab17749c7b1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5cc03a916aa7a1a7160aab17749c7b1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4be42b28ba4bdb04ec250ac5a1d23335.jpg\" _src=\"http://yanxuan.nosdn.127.net/4be42b28ba4bdb04ec250ac5a1d23335.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f1f5bf21475bc50979dce49894bd03c.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f1f5bf21475bc50979dce49894bd03c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dca09a7be97a3bbebeea80f6266e1cbe.jpg\" _src=\"http://yanxuan.nosdn.127.net/dca09a7be97a3bbebeea80f6266e1cbe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82cfe49a34dd57e9879ab264b2c4a0f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/82cfe49a34dd57e9879ab264b2c4a0f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/609766611ba2b7f471f4b5ec3cfb1570.jpg\" _src=\"http://yanxuan.nosdn.127.net/609766611ba2b7f471f4b5ec3cfb1570.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b4bfa751387777262f0dd3cbfeda6cf3.jpg\" _src=\"http://yanxuan.nosdn.127.net/b4bfa751387777262f0dd3cbfeda6cf3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cce5ecbcc8d6cbaf2da11a0efa137467.jpg\" _src=\"http://yanxuan.nosdn.127.net/cce5ecbcc8d6cbaf2da11a0efa137467.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0d698dd6bad6abd7b5ad731ca8954ab9.jpg\" _src=\"http://yanxuan.nosdn.127.net/0d698dd6bad6abd7b5ad731ca8954ab9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/34b463871aee608c1c3ccc9a6ae4e7fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/34b463871aee608c1c3ccc9a6ae4e7fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6d7d047d324a9878de7cc1ccd2b24fab.jpg\" _src=\"http://yanxuan.nosdn.127.net/6d7d047d324a9878de7cc1ccd2b24fab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf43f53d3770ff5d34eaade48c42ddf0.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf43f53d3770ff5d34eaade48c42ddf0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e4d8478f1cbe72b6991e59cdbf2c1c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e4d8478f1cbe72b6991e59cdbf2c1c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec91680fb9913afc597afc4295c9810e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec91680fb9913afc597afc4295c9810e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf5f83c67d2b6303fc10d7698211c451.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf5f83c67d2b6303fc10d7698211c451.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c4e736beeba84fa508b5001c14326817.jpg\" _src=\"http://yanxuan.nosdn.127.net/c4e736beeba84fa508b5001c14326817.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b39bb20bc10eb80a4a73af1ef72e1f14.jpg\" _src=\"http://yanxuan.nosdn.127.net/b39bb20bc10eb80a4a73af1ef72e1f14.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ee97cc8179dc8f63df9545ed4cf1289.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ee97cc8179dc8f63df9545ed4cf1289.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b6f5d89595f271bf1ece37ef1a59b7fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/b6f5d89595f271bf1ece37ef1a59b7fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cfc8924f6085deaf154deb6da8ac794.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cfc8924f6085deaf154deb6da8ac794.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69dc1813268f768aa90f696807c0614c.jpg\" _src=\"http://yanxuan.nosdn.127.net/69dc1813268f768aa90f696807c0614c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a781da27715d6bbb246e7a9997e1ef4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/a781da27715d6bbb246e7a9997e1ef4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e3177e5434d5ef56ea7a782358da8ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e3177e5434d5ef56ea7a782358da8ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/64468f6698d122f7c554299af3ea9f13.jpg\" _src=\"http://yanxuan.nosdn.127.net/64468f6698d122f7c554299af3ea9f13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/024b2a81d2860e631165a80a7142cf67.jpg\" _src=\"http://yanxuan.nosdn.127.net/024b2a81d2860e631165a80a7142cf67.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85b12419b868dc311361781e50d46877.jpg\" _src=\"http://yanxuan.nosdn.127.net/85b12419b868dc311361781e50d46877.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6fcff064127cdf5b5a73d358db4efa21.jpg\" _src=\"http://yanxuan.nosdn.127.net/6fcff064127cdf5b5a73d358db4efa21.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f28c8dd3c027fbfd64952d2c55b87fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f28c8dd3c027fbfd64952d2c55b87fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/144ee76547f7b21bacb763426af25f07.jpg\" _src=\"http://yanxuan.nosdn.127.net/144ee76547f7b21bacb763426af25f07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/191c12adb5895f7fb71c9d5b8bee424d.jpg\" _src=\"http://yanxuan.nosdn.127.net/191c12adb5895f7fb71c9d5b8bee424d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7158e3fa0c0c034b91dbd06d2eccef3a.jpg\" _src=\"http://yanxuan.nosdn.127.net/7158e3fa0c0c034b91dbd06d2eccef3a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/01da4634f8486926944213e12b15e114.jpg\" _src=\"http://yanxuan.nosdn.127.net/01da4634f8486926944213e12b15e114.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/957eaa7ec5510cfc24d41e82f0882406.jpg\" _src=\"http://yanxuan.nosdn.127.net/957eaa7ec5510cfc24d41e82f0882406.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 20,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a8435686775f39284c0976d9cd8490ef.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ce4a1eb18ea518bf584620632509935f.png",
      "retail_price": 2399,
      "sell_volume": 607,
      "primary_product_id": 1079056,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1090004,
      "category_id": 1008009,
      "goods_sn": "1090004",
      "name": "日式法兰绒格子四件套",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "气质英伦格纹，法兰绒的丰满细腻",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/c5d674aa299a695c5c4c0db81025e754.jpg\" _src=\"http://yanxuan.nosdn.127.net/c5d674aa299a695c5c4c0db81025e754.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f26e78d93e29aab32b4629dc0ac46a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f26e78d93e29aab32b4629dc0ac46a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f56ec00fd8014106cf25a661d3ec797b.jpg\" _src=\"http://yanxuan.nosdn.127.net/f56ec00fd8014106cf25a661d3ec797b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/74ee09e3d121c21c128fda3dbb48ff93.jpg\" _src=\"http://yanxuan.nosdn.127.net/74ee09e3d121c21c128fda3dbb48ff93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b6a5cb5e75cc5159ef19e68a68c571f.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b6a5cb5e75cc5159ef19e68a68c571f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d046159b8b5940565e52d432af47fdf.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d046159b8b5940565e52d432af47fdf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ea5cebdcf5c5b6c7b63c537c391fac0.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ea5cebdcf5c5b6c7b63c537c391fac0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbe2aa2c6f479f1a2fa7c3d1168eb2da.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbe2aa2c6f479f1a2fa7c3d1168eb2da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c83ea824cd0baea85933c1a7ab7a6391.jpg\" _src=\"http://yanxuan.nosdn.127.net/c83ea824cd0baea85933c1a7ab7a6391.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1fcea29ea7aee7b8547dab203a2f0a2e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1fcea29ea7aee7b8547dab203a2f0a2e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/303e723e88c7a97637b03e8b6c909228.jpg\" _src=\"http://yanxuan.nosdn.127.net/303e723e88c7a97637b03e8b6c909228.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/45f6d6f44148d26fda2d433b8996a023.jpg\" _src=\"http://yanxuan.nosdn.127.net/45f6d6f44148d26fda2d433b8996a023.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b02c994370c16d506b2816323963a05.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b02c994370c16d506b2816323963a05.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/13b1c59a181c003ef49c089697162f11.jpg\" _src=\"http://yanxuan.nosdn.127.net/13b1c59a181c003ef49c089697162f11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9066da74fa3268749af74d48583a3915.jpg\" _src=\"http://yanxuan.nosdn.127.net/9066da74fa3268749af74d48583a3915.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22d1cbe72022eeefabdebb881be7be53.jpg\" _src=\"http://yanxuan.nosdn.127.net/22d1cbe72022eeefabdebb881be7be53.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cdc0bb9e30e01729ef23564b07cffe45.jpg\" _src=\"http://yanxuan.nosdn.127.net/cdc0bb9e30e01729ef23564b07cffe45.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6249c39ca733c75bc8c0bb90daeeb12a.jpg\" _src=\"http://yanxuan.nosdn.127.net/6249c39ca733c75bc8c0bb90daeeb12a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f70749f36b60bd1962ce28ed180a93e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/f70749f36b60bd1962ce28ed180a93e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c55fa3317e09fe3d3e2971f768e00947.jpg\" _src=\"http://yanxuan.nosdn.127.net/c55fa3317e09fe3d3e2971f768e00947.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3477d90873d80315571165816991a2e.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3477d90873d80315571165816991a2e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5c24363b2cd4728d0c0ef19478bda3f5.jpg\" _src=\"http://yanxuan.nosdn.127.net/5c24363b2cd4728d0c0ef19478bda3f5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b92e6be5e80ff4cf55d06b284ab784ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/b92e6be5e80ff4cf55d06b284ab784ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7137ebf6468571550adaa70a3c770eb.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7137ebf6468571550adaa70a3c770eb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88b466104d4d8502c28029bd8a5852ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/88b466104d4d8502c28029bd8a5852ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ccf54b36177613093209b78d992f50af.jpg\" _src=\"http://yanxuan.nosdn.127.net/ccf54b36177613093209b78d992f50af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb37be13750edf70aec43d9be731eb10.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb37be13750edf70aec43d9be731eb10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cdb3ef4a50634629885d163e8b91d71.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cdb3ef4a50634629885d163e8b91d71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/24e991af9b9704ff1b2963fd2e999763.jpg\" _src=\"http://yanxuan.nosdn.127.net/24e991af9b9704ff1b2963fd2e999763.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77250c6dbf13b1b2955bf2f9ae44b454.jpg\" _src=\"http://yanxuan.nosdn.127.net/77250c6dbf13b1b2955bf2f9ae44b454.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7dedee5ad49f66f01f88c8cd94786c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7dedee5ad49f66f01f88c8cd94786c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c302e07c426c207a88ab703fda7f244.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c302e07c426c207a88ab703fda7f244.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5285d43ecccf0d28afcacccdc3054461.jpg\" _src=\"http://yanxuan.nosdn.127.net/5285d43ecccf0d28afcacccdc3054461.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/24cc9d53907a67ee5564611f9649121f.jpg\" _src=\"http://yanxuan.nosdn.127.net/24cc9d53907a67ee5564611f9649121f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad70628c1f27db2afa22874e9fad72e0.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad70628c1f27db2afa22874e9fad72e0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89277ed3ec4b8c34ae027c33d61cac53.jpg\" _src=\"http://yanxuan.nosdn.127.net/89277ed3ec4b8c34ae027c33d61cac53.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff64316933f4fa3b0991f2ddeff84f91.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff64316933f4fa3b0991f2ddeff84f91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/201299d3c5ec454b605b1ea23259a999.jpg\" _src=\"http://yanxuan.nosdn.127.net/201299d3c5ec454b605b1ea23259a999.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/471c49adb955692d6bf571ec78a45bed.jpg\" _src=\"http://yanxuan.nosdn.127.net/471c49adb955692d6bf571ec78a45bed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53b525a3b77c6a51a0f2629e1d4cec79.jpg\" _src=\"http://yanxuan.nosdn.127.net/53b525a3b77c6a51a0f2629e1d4cec79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10ed5f6502699bd5dbf451cf503f91a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/10ed5f6502699bd5dbf451cf503f91a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84b29a0e3877ce6a0c536e7de9451987.jpg\" _src=\"http://yanxuan.nosdn.127.net/84b29a0e3877ce6a0c536e7de9451987.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9518254ccd271857e43d5ebf8fa16cc9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9518254ccd271857e43d5ebf8fa16cc9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8eda4c6e16f647c122c8e1fb72a5c296.jpg\" _src=\"http://yanxuan.nosdn.127.net/8eda4c6e16f647c122c8e1fb72a5c296.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9fa5cfdb4911b91bbb1ed617809dfd74.jpg\" _src=\"http://yanxuan.nosdn.127.net/9fa5cfdb4911b91bbb1ed617809dfd74.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d5849257871c8cdd4cb35e8e012b4da.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d5849257871c8cdd4cb35e8e012b4da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29ad636afec8d03bda3074611b8b4a2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/29ad636afec8d03bda3074611b8b4a2d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/163404e599ff0fd71396efaabb32f660.jpg\" _src=\"http://yanxuan.nosdn.127.net/163404e599ff0fd71396efaabb32f660.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7189a89979d51090a2c2492b716634f.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7189a89979d51090a2c2492b716634f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d28aaf8c345118e16742dde54f2a70e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/d28aaf8c345118e16742dde54f2a70e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e31e9df5a49f85cc18676f4ce97d118.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e31e9df5a49f85cc18676f4ce97d118.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7aaed516f1280e923796c46b364fbc20.jpg\" _src=\"http://yanxuan.nosdn.127.net/7aaed516f1280e923796c46b364fbc20.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bbb2299807545f2c96717276feb200a.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bbb2299807545f2c96717276feb200a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b6b989f53d9c5d9d5046226000c2f8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b6b989f53d9c5d9d5046226000c2f8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9a04c82669e08d0f884db98a63d2d268.jpg\" _src=\"http://yanxuan.nosdn.127.net/9a04c82669e08d0f884db98a63d2d268.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19e6c5e17ed0490eb761c4e9cc207d13.jpg\" _src=\"http://yanxuan.nosdn.127.net/19e6c5e17ed0490eb761c4e9cc207d13.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 17,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/32ba9417c9d31c6ea686ec842df3ca61.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/a3a92057f10e5e6e804c19ef495e3dee.png",
      "retail_price": 399,
      "sell_volume": 2156,
      "primary_product_id": 1095010,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1109008,
      "category_id": 1015000,
      "goods_sn": "1109008",
      "name": "云端沙发组合",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "MUJI供应商携手打造",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/fc48d623ad2effc32f47f70e6cba03ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/fc48d623ad2effc32f47f70e6cba03ee.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb4a737f74e7779d19c998a0ba63cd3d.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb4a737f74e7779d19c998a0ba63cd3d.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/937038be185fc64572c38de8d69c01cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/937038be185fc64572c38de8d69c01cb.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40108d88fbfe752bfb7a6fc4ae8edd79.jpg\" _src=\"http://yanxuan.nosdn.127.net/40108d88fbfe752bfb7a6fc4ae8edd79.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a28a0420050289d3e19b88d28b76bab6.jpg\" _src=\"http://yanxuan.nosdn.127.net/a28a0420050289d3e19b88d28b76bab6.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/917acd26520c10b3c82d2beed37fddd7.jpg\" _src=\"http://yanxuan.nosdn.127.net/917acd26520c10b3c82d2beed37fddd7.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbf4e7008c33239f7cf79aa93f68ee15.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbf4e7008c33239f7cf79aa93f68ee15.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54065646ecdae5f010980bfa24c4fbbe.jpg\" _src=\"http://yanxuan.nosdn.127.net/54065646ecdae5f010980bfa24c4fbbe.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff510e36a124d4c1ccce47a1e06cba30.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff510e36a124d4c1ccce47a1e06cba30.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b33aa96ae830fec44aac042f1f28ddd8.jpg\" _src=\"http://yanxuan.nosdn.127.net/b33aa96ae830fec44aac042f1f28ddd8.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff74ec438ab3d7805ea2aed2c6552746.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff74ec438ab3d7805ea2aed2c6552746.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6eaff5f5a38874a6e2a9b56feeede7d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/6eaff5f5a38874a6e2a9b56feeede7d7.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/200c9aae4e02a75bd71a5dea29f726c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/200c9aae4e02a75bd71a5dea29f726c4.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cd48b3606d7bb30243eebded22617d2e.jpg\" _src=\"http://yanxuan.nosdn.127.net/cd48b3606d7bb30243eebded22617d2e.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bcc453ac7a81cfc517a192ff00013745.jpg\" _src=\"http://yanxuan.nosdn.127.net/bcc453ac7a81cfc517a192ff00013745.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5a4e50f5936b3c0ec5b163c8ccc99e8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/5a4e50f5936b3c0ec5b163c8ccc99e8a.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a79d51d47fadefe7b7db72052d98337f.jpg\" _src=\"http://yanxuan.nosdn.127.net/a79d51d47fadefe7b7db72052d98337f.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ed0d597c81b9ec49b969f8357eac8bd.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ed0d597c81b9ec49b969f8357eac8bd.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/177f0b2f78bcccf6926c47eb7ef2b047.jpg\" _src=\"http://yanxuan.nosdn.127.net/177f0b2f78bcccf6926c47eb7ef2b047.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/808241e6912a1015f94da67d80a296cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/808241e6912a1015f94da67d80a296cf.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a123c112a75dee43559674c680c941ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/a123c112a75dee43559674c680c941ae.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/832eefe1435ceeaeb421ce7ec0a4fa51.jpg\" _src=\"http://yanxuan.nosdn.127.net/832eefe1435ceeaeb421ce7ec0a4fa51.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b6f1a00452bc026eba362e4a1d58e04.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b6f1a00452bc026eba362e4a1d58e04.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/761f4fadf4c797affe42c125b29c8ec9.jpg\" _src=\"http://yanxuan.nosdn.127.net/761f4fadf4c797affe42c125b29c8ec9.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d927eded8a39bbb888f9994cd236cb56.jpg\" _src=\"http://yanxuan.nosdn.127.net/d927eded8a39bbb888f9994cd236cb56.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70c47dd65c21bd3fe52f179480268b54.jpg\" _src=\"http://yanxuan.nosdn.127.net/70c47dd65c21bd3fe52f179480268b54.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02a226a867d397c20aafae1f5449225c.jpg\" _src=\"http://yanxuan.nosdn.127.net/02a226a867d397c20aafae1f5449225c.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76c8f1702e4c8f1072eb1cba6776f7c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/76c8f1702e4c8f1072eb1cba6776f7c7.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/36225b551bb1e85691f29aa040ab9497.jpg\" _src=\"http://yanxuan.nosdn.127.net/36225b551bb1e85691f29aa040ab9497.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d9ba3ce28d578267765c4d2bc62b887.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d9ba3ce28d578267765c4d2bc62b887.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/099296fb5f8e88ab1c5eaffbd37b8c70.jpg\" _src=\"http://yanxuan.nosdn.127.net/099296fb5f8e88ab1c5eaffbd37b8c70.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bce3a4f414e16497dd0a1301fe945732.jpg\" _src=\"http://yanxuan.nosdn.127.net/bce3a4f414e16497dd0a1301fe945732.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e75874726dd5a742599bc96f4401b51a.jpg\" _src=\"http://yanxuan.nosdn.127.net/e75874726dd5a742599bc96f4401b51a.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cf202434f6e7d84388eb3f00aef3cf7.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cf202434f6e7d84388eb3f00aef3cf7.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2788c15d1fb4b12ea989b4626bf4dd42.jpg\" _src=\"http://yanxuan.nosdn.127.net/2788c15d1fb4b12ea989b4626bf4dd42.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/988c7843cd5e3c3d41ded3f964e83f28.jpg\" _src=\"http://yanxuan.nosdn.127.net/988c7843cd5e3c3d41ded3f964e83f28.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8680210644f9ddacc776c086acf087c.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8680210644f9ddacc776c086acf087c.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/06a5234e14a9a5a13cab234e338ee047.jpg\" _src=\"http://yanxuan.nosdn.127.net/06a5234e14a9a5a13cab234e338ee047.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6913fa996a08d015baa5dbb81c6751b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/6913fa996a08d015baa5dbb81c6751b4.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5559938dfbba2abfe6dc2905892048d6.jpg\" _src=\"http://yanxuan.nosdn.127.net/5559938dfbba2abfe6dc2905892048d6.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3bd6c290baf02cd9d6e8f2036ad96055.jpg\" _src=\"http://yanxuan.nosdn.127.net/3bd6c290baf02cd9d6e8f2036ad96055.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c13f0abbe2e7c8bb6d78986dcaca45a8.jpg\" _src=\"http://yanxuan.nosdn.127.net/c13f0abbe2e7c8bb6d78986dcaca45a8.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38d1037057ffb3642d518415c3c21400.jpg\" _src=\"http://yanxuan.nosdn.127.net/38d1037057ffb3642d518415c3c21400.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8f56ea468a1a9fc4dbb462be94b0167.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8f56ea468a1a9fc4dbb462be94b0167.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f47f956787047fc4c05107beef0fd15b.jpg\" _src=\"http://yanxuan.nosdn.127.net/f47f956787047fc4c05107beef0fd15b.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59ae5ce70d03639554b3e0d222416de1.jpg\" _src=\"http://yanxuan.nosdn.127.net/59ae5ce70d03639554b3e0d222416de1.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e54c9882590f3dc3524229c190098b7.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e54c9882590f3dc3524229c190098b7.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb714d5f8e9c3a0cbb063f492c94a9a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb714d5f8e9c3a0cbb063f492c94a9a7.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afdf2db3aeababc5e2eacbe3e03ab505.jpg\" _src=\"http://yanxuan.nosdn.127.net/afdf2db3aeababc5e2eacbe3e03ab505.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e4b140b65d6da223b2e43082640715e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e4b140b65d6da223b2e43082640715e.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0a4feb902cbd98370508538d252985c2.jpg\" _src=\"http://yanxuan.nosdn.127.net/0a4feb902cbd98370508538d252985c2.jpg\"/></p><p style=\"text-align: center;\"><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 2,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2230e0d14986e273fb310269a0eb075c.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/c5be2604c0e4186a4e7079feeb742cee.png",
      "retail_price": 3999,
      "sell_volume": 274,
      "primary_product_id": 1110009,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1110003,
      "category_id": 1008009,
      "goods_sn": "1110003",
      "name": "全棉针织条纹四件套 新款",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "裸睡享受，柔软透气有弹性",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/51409b5b30124fcef4b15ae9bd3d1047.jpg\" _src=\"http://yanxuan.nosdn.127.net/51409b5b30124fcef4b15ae9bd3d1047.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ed3bbf85dc26140e5b054ea5ff8aa28.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ed3bbf85dc26140e5b054ea5ff8aa28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1486e921307df5cbaf21f27d2ffb4404.jpg\" _src=\"http://yanxuan.nosdn.127.net/1486e921307df5cbaf21f27d2ffb4404.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8692330cd1abc6317f090ccd5d28bf9f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8692330cd1abc6317f090ccd5d28bf9f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e046657e9f8b523c0cd93d2fbbe566c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e046657e9f8b523c0cd93d2fbbe566c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2ca5a528cfd0c24bb97aed0c1a2fe35.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2ca5a528cfd0c24bb97aed0c1a2fe35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a0087be757bbb5070a9495cf32d2d7a4.jpg\" _src=\"http://yanxuan.nosdn.127.net/a0087be757bbb5070a9495cf32d2d7a4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bce9b677188a36b86fa40e13011a43a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/bce9b677188a36b86fa40e13011a43a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6a0a90deb515f06d8d1c275c2057e368.jpg\" _src=\"http://yanxuan.nosdn.127.net/6a0a90deb515f06d8d1c275c2057e368.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39d50a3a61d13163bf83774edd2db5bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/39d50a3a61d13163bf83774edd2db5bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/408ae6a44271a7fec18dcaaa66a66d2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/408ae6a44271a7fec18dcaaa66a66d2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/033fd7aed18e0fcd50ea695239fdf5d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/033fd7aed18e0fcd50ea695239fdf5d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/519ddc7d3c063973fbd221a8bf9fb62c.jpg\" _src=\"http://yanxuan.nosdn.127.net/519ddc7d3c063973fbd221a8bf9fb62c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4855bf5174f5a9c59ff92b134a9c6702.jpg\" _src=\"http://yanxuan.nosdn.127.net/4855bf5174f5a9c59ff92b134a9c6702.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2a6d73ee470dfc663b1ef7f45d25f0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2a6d73ee470dfc663b1ef7f45d25f0e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a59172ea5938721b3a5a66b049bc31a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a59172ea5938721b3a5a66b049bc31a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8c29ecaa289359d6a9ee0f553e512902.jpg\" _src=\"http://yanxuan.nosdn.127.net/8c29ecaa289359d6a9ee0f553e512902.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/717bff823050ff266da8e0ae04eae1cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/717bff823050ff266da8e0ae04eae1cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1de5768520db342444d3cb620a9fdd4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1de5768520db342444d3cb620a9fdd4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/453b37dfd7b3ae539f7afb7e3d3fda73.jpg\" _src=\"http://yanxuan.nosdn.127.net/453b37dfd7b3ae539f7afb7e3d3fda73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29a9b2ac9aa56666fafd4c90b1a7fed1.jpg\" _src=\"http://yanxuan.nosdn.127.net/29a9b2ac9aa56666fafd4c90b1a7fed1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8a15810a575de26a33a5ac9983c68939.jpg\" _src=\"http://yanxuan.nosdn.127.net/8a15810a575de26a33a5ac9983c68939.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbe607ff748b140e02946bb28578a179.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbe607ff748b140e02946bb28578a179.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02e0e40e7423fbf85ad31ccb483b519b.jpg\" _src=\"http://yanxuan.nosdn.127.net/02e0e40e7423fbf85ad31ccb483b519b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a352d098862cc87a3de60a42147896f.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a352d098862cc87a3de60a42147896f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b783bbe92f495b5d1095afe96d2a3685.jpg\" _src=\"http://yanxuan.nosdn.127.net/b783bbe92f495b5d1095afe96d2a3685.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a55100ca3526614393371f7f3a466dda.jpg\" _src=\"http://yanxuan.nosdn.127.net/a55100ca3526614393371f7f3a466dda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e40fb00aec446ed6695e25d458b4a1bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/e40fb00aec446ed6695e25d458b4a1bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23481a0858e9d4a62a5b707c6b3f8f4b.jpg\" _src=\"http://yanxuan.nosdn.127.net/23481a0858e9d4a62a5b707c6b3f8f4b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a25526218ef089322f56b69dc12e14af.jpg\" _src=\"http://yanxuan.nosdn.127.net/a25526218ef089322f56b69dc12e14af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7c752cfaedadc0687c5774e00a760dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7c752cfaedadc0687c5774e00a760dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/234a67ee6018ceb8660695e662fabb99.jpg\" _src=\"http://yanxuan.nosdn.127.net/234a67ee6018ceb8660695e662fabb99.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/174b1bb41003bcddd8dc9c9ef17ce224.jpg\" _src=\"http://yanxuan.nosdn.127.net/174b1bb41003bcddd8dc9c9ef17ce224.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abd9fea1d638e7a5aecc6a7adc76c711.jpg\" _src=\"http://yanxuan.nosdn.127.net/abd9fea1d638e7a5aecc6a7adc76c711.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e08f5def5de99f8bebe3ec6a1ae1c83.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e08f5def5de99f8bebe3ec6a1ae1c83.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2995438e191249bd7d084a5d6f2373c8.jpg\" _src=\"http://yanxuan.nosdn.127.net/2995438e191249bd7d084a5d6f2373c8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb07fd94e9566b69757833b2633b28df.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb07fd94e9566b69757833b2633b28df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8fca21912470098294ec527ea245821.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8fca21912470098294ec527ea245821.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32f2e9e3f2b68c131e3219df1d2abda0.jpg\" _src=\"http://yanxuan.nosdn.127.net/32f2e9e3f2b68c131e3219df1d2abda0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/808917d73d100f81297b133b14976a2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/808917d73d100f81297b133b14976a2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9af0fe13111566c77485e3be2151059.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9af0fe13111566c77485e3be2151059.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/122464e4981f97f4ddb18a56e4eaae52.jpg\" _src=\"http://yanxuan.nosdn.127.net/122464e4981f97f4ddb18a56e4eaae52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abc8125353e8c485f68eecde6e49dddb.jpg\" _src=\"http://yanxuan.nosdn.127.net/abc8125353e8c485f68eecde6e49dddb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8ba0e58c2ff94139b3d808c33f907a4.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8ba0e58c2ff94139b3d808c33f907a4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6134c0363c2861e9dc0b1244eaf8cf85.jpg\" _src=\"http://yanxuan.nosdn.127.net/6134c0363c2861e9dc0b1244eaf8cf85.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fe8ed929bbf2f23b09b8359c846fbdf.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fe8ed929bbf2f23b09b8359c846fbdf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/94cf259d560b3f0d53603d261ad47d69.jpg\" _src=\"http://yanxuan.nosdn.127.net/94cf259d560b3f0d53603d261ad47d69.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d14cd06d113b7053bbc416fce83e6ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d14cd06d113b7053bbc416fce83e6ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a57ce45eccdc407c6d87d515d64c9d0f.jpg\" _src=\"http://yanxuan.nosdn.127.net/a57ce45eccdc407c6d87d515d64c9d0f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d339a7656c240792d234e3edbb1bdd6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/d339a7656c240792d234e3edbb1bdd6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f18f868fdf16912d4e89f3421fffec65.jpg\" _src=\"http://yanxuan.nosdn.127.net/f18f868fdf16912d4e89f3421fffec65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f2bae908dc57231874edb377b95e6d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f2bae908dc57231874edb377b95e6d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/efeb13be9fb6664625f37e639ec9cf67.jpg\" _src=\"http://yanxuan.nosdn.127.net/efeb13be9fb6664625f37e639ec9cf67.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c82da9f8e4b68ef552878a0ef8160e12.jpg\" _src=\"http://yanxuan.nosdn.127.net/c82da9f8e4b68ef552878a0ef8160e12.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77db454604d83b15ed289604ac0c6282.jpg\" _src=\"http://yanxuan.nosdn.127.net/77db454604d83b15ed289604ac0c6282.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a5def4bad25b8f0105621f6151b20f29.jpg\" _src=\"http://yanxuan.nosdn.127.net/a5def4bad25b8f0105621f6151b20f29.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1204e404c87dad014daebe47946c642a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1204e404c87dad014daebe47946c642a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85165ab6336f96477b5ed4f40c1f4506.jpg\" _src=\"http://yanxuan.nosdn.127.net/85165ab6336f96477b5ed4f40c1f4506.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76d0a15612658df2da7f90141c27575b.jpg\" _src=\"http://yanxuan.nosdn.127.net/76d0a15612658df2da7f90141c27575b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18d88fcaa7184e70a3fe2af7a410ea92.jpg\" _src=\"http://yanxuan.nosdn.127.net/18d88fcaa7184e70a3fe2af7a410ea92.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 2,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/eeba45c72fa097c6e128d529b7a0c513.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/72dfb4bfc1cd1b834c064a9d1d40627d.png",
      "retail_price": 299,
      "sell_volume": 19852,
      "primary_product_id": 1111023,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1110004,
      "category_id": 1008009,
      "goods_sn": "1110004",
      "name": "全棉针织纯色四件套",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "日系纯色，面料轻柔舒透",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/e15427b1300012152bf9d92a2bc67c99.jpg\" _src=\"http://yanxuan.nosdn.127.net/e15427b1300012152bf9d92a2bc67c99.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7428b57cf1524e25e868046a52c8c74.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7428b57cf1524e25e868046a52c8c74.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ba73e0fac1ddac61dac545147360f30.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ba73e0fac1ddac61dac545147360f30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2132694338933fdce383149a883680ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/2132694338933fdce383149a883680ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/06f8db4f9ec0c46aa369e3a47334fdf6.jpg\" _src=\"http://yanxuan.nosdn.127.net/06f8db4f9ec0c46aa369e3a47334fdf6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/98ea40eb0129d0e9d8152d5db6f826a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/98ea40eb0129d0e9d8152d5db6f826a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/450133053e1e892623b0c66522e4cd13.jpg\" _src=\"http://yanxuan.nosdn.127.net/450133053e1e892623b0c66522e4cd13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/266fe2d8d8284830ce353b717b134006.jpg\" _src=\"http://yanxuan.nosdn.127.net/266fe2d8d8284830ce353b717b134006.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e79e83d77a24109e4e571e8bb327489.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e79e83d77a24109e4e571e8bb327489.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e7c40f873354dd00827a8e9a116ae9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e7c40f873354dd00827a8e9a116ae9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd63c2c2c421d9ae62e42378531eb9bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd63c2c2c421d9ae62e42378531eb9bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5d5fb2641ad2011b304a839dccfaceb.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5d5fb2641ad2011b304a839dccfaceb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e44ecb22b4288445c73348aee7848e74.jpg\" _src=\"http://yanxuan.nosdn.127.net/e44ecb22b4288445c73348aee7848e74.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff2b9e9b6d07861e53c535de160c89b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff2b9e9b6d07861e53c535de160c89b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbd8db78cccec3b459cefc8403977565.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbd8db78cccec3b459cefc8403977565.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d33fa09d06e55946ed3ca575e1ac8ca.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d33fa09d06e55946ed3ca575e1ac8ca.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/710e44a757e0af28923c6d8451729f9d.jpg\" _src=\"http://yanxuan.nosdn.127.net/710e44a757e0af28923c6d8451729f9d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83fd15d26c23b24cdb85b56552ec1f60.jpg\" _src=\"http://yanxuan.nosdn.127.net/83fd15d26c23b24cdb85b56552ec1f60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a6aa91581b046928b799a84f0871d6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a6aa91581b046928b799a84f0871d6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92c89ac95e0681e11f04772e5f1fb55c.jpg\" _src=\"http://yanxuan.nosdn.127.net/92c89ac95e0681e11f04772e5f1fb55c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80b35361b1896d38260c3d1982c462ff.jpg\" _src=\"http://yanxuan.nosdn.127.net/80b35361b1896d38260c3d1982c462ff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eee8f49786481c7ea533e8315c743f96.jpg\" _src=\"http://yanxuan.nosdn.127.net/eee8f49786481c7ea533e8315c743f96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84eebca8658c8ed824c1b04ea5ce0262.jpg\" _src=\"http://yanxuan.nosdn.127.net/84eebca8658c8ed824c1b04ea5ce0262.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a17beea5ce5e36f1de3e28121b3bf90.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a17beea5ce5e36f1de3e28121b3bf90.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a6587bb904df455610f3e2893b403ff6.jpg\" _src=\"http://yanxuan.nosdn.127.net/a6587bb904df455610f3e2893b403ff6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62d1faf12c878f8f8d0f6f90816f82eb.jpg\" _src=\"http://yanxuan.nosdn.127.net/62d1faf12c878f8f8d0f6f90816f82eb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/64b1010703632d102692f1cfdc329c07.jpg\" _src=\"http://yanxuan.nosdn.127.net/64b1010703632d102692f1cfdc329c07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ee9a6bd5a6d345274dfc5bd3df8f6673.jpg\" _src=\"http://yanxuan.nosdn.127.net/ee9a6bd5a6d345274dfc5bd3df8f6673.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/924b2879cd336d3fcc5c2dd064fa563d.jpg\" _src=\"http://yanxuan.nosdn.127.net/924b2879cd336d3fcc5c2dd064fa563d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5627b5789c5faeb6f2f0eb319d4eb758.jpg\" _src=\"http://yanxuan.nosdn.127.net/5627b5789c5faeb6f2f0eb319d4eb758.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a6125e2c756374638db2cff6e1f1834d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a6125e2c756374638db2cff6e1f1834d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7c65c61453f6503723ca73b502b3d89.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7c65c61453f6503723ca73b502b3d89.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9d7b28b69a8c75f0a30a9753126d03c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9d7b28b69a8c75f0a30a9753126d03c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54841f38fc0883cd9ab86ac7b8345801.jpg\" _src=\"http://yanxuan.nosdn.127.net/54841f38fc0883cd9ab86ac7b8345801.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8703301aa06b22d2d6699745f9b15770.jpg\" _src=\"http://yanxuan.nosdn.127.net/8703301aa06b22d2d6699745f9b15770.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c824bc7de6471d1b07797d3c6f77a33d.jpg\" _src=\"http://yanxuan.nosdn.127.net/c824bc7de6471d1b07797d3c6f77a33d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ce29e7160e862b4c55acb51734bbf30.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ce29e7160e862b4c55acb51734bbf30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/220774e0cdc07e4448af3cb650c398eb.jpg\" _src=\"http://yanxuan.nosdn.127.net/220774e0cdc07e4448af3cb650c398eb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d660bb8f822d9f5fa9eeb2cad568ae0c.jpg\" _src=\"http://yanxuan.nosdn.127.net/d660bb8f822d9f5fa9eeb2cad568ae0c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dfe8564614a61d7b040c02565211c77.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dfe8564614a61d7b040c02565211c77.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8b6f2ad58a4f4d159580362e4dc7625.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8b6f2ad58a4f4d159580362e4dc7625.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f42bd22e79764026659e48e40c131353.jpg\" _src=\"http://yanxuan.nosdn.127.net/f42bd22e79764026659e48e40c131353.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/298706644d4d54146d693bb69d0972bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/298706644d4d54146d693bb69d0972bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d77bdd18e48fd17010ebbb825bb52dcf.jpg\" _src=\"http://yanxuan.nosdn.127.net/d77bdd18e48fd17010ebbb825bb52dcf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a11788ef69114eddb1dcdf4d9f8320e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/a11788ef69114eddb1dcdf4d9f8320e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c36bce03ee7386ff09f913bbf0eff163.jpg\" _src=\"http://yanxuan.nosdn.127.net/c36bce03ee7386ff09f913bbf0eff163.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/481edda8c381a26f138e2785714de72b.jpg\" _src=\"http://yanxuan.nosdn.127.net/481edda8c381a26f138e2785714de72b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0d8999ba08cb6002401523e55214a8fe.jpg\" _src=\"http://yanxuan.nosdn.127.net/0d8999ba08cb6002401523e55214a8fe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4ae747c627f5a530dd1defad463fda5f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4ae747c627f5a530dd1defad463fda5f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5bb1d2df0e1e9a9713aaa4fd534f9613.jpg\" _src=\"http://yanxuan.nosdn.127.net/5bb1d2df0e1e9a9713aaa4fd534f9613.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89bfd74e9a71117724edef87fd9d3729.jpg\" _src=\"http://yanxuan.nosdn.127.net/89bfd74e9a71117724edef87fd9d3729.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d9eb35c8b7fb88bf15352b9586b93f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d9eb35c8b7fb88bf15352b9586b93f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/400146bec77d8d243332c1e53a903839.jpg\" _src=\"http://yanxuan.nosdn.127.net/400146bec77d8d243332c1e53a903839.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d1c6b1cf18f2bf441aa90768aff1833a.jpg\" _src=\"http://yanxuan.nosdn.127.net/d1c6b1cf18f2bf441aa90768aff1833a.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 3,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/65d94c770e03dacd4e1b8b45ad481e55.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/1ffd5831e63027715445f74a28f8c4ed.png",
      "retail_price": 299,
      "sell_volume": 11983,
      "primary_product_id": 1111037,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1110007,
      "category_id": 1008009,
      "goods_sn": "1110007",
      "name": "日式色织水洗棉格纹四件套 新款",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "做旧微褶感，轻柔呵护棉",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/280d74c31b9322eb956e7481bd22e9a5.jpg\" _src=\"http://yanxuan.nosdn.127.net/280d74c31b9322eb956e7481bd22e9a5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2b9270ec5d66c917f2514f8d69679f6c.jpg\" _src=\"http://yanxuan.nosdn.127.net/2b9270ec5d66c917f2514f8d69679f6c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5126fea2c070ab454df529b7cd42171a.jpg\" _src=\"http://yanxuan.nosdn.127.net/5126fea2c070ab454df529b7cd42171a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7020173bf8664bae6a51ec81a5045350.jpg\" _src=\"http://yanxuan.nosdn.127.net/7020173bf8664bae6a51ec81a5045350.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f68d38ae6dfe3b56c3e0ddf4446105e.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f68d38ae6dfe3b56c3e0ddf4446105e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e401c41d6e3cc2ad655383fb83f582e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/e401c41d6e3cc2ad655383fb83f582e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6e0801c89d5119c02f4aad1fa2e3f79d.jpg\" _src=\"http://yanxuan.nosdn.127.net/6e0801c89d5119c02f4aad1fa2e3f79d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb11f89e6f0c41053087f0b4bbed36c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb11f89e6f0c41053087f0b4bbed36c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80bf0c6ef68f4373b3db521e7c09f0fb.jpg\" _src=\"http://yanxuan.nosdn.127.net/80bf0c6ef68f4373b3db521e7c09f0fb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ec681b58c2b2281ceac667bb9416e79.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ec681b58c2b2281ceac667bb9416e79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab6e782785293c93cddbbe59d41fbe58.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab6e782785293c93cddbbe59d41fbe58.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2974fb17474f1e75a3746cbdb9d38d08.jpg\" _src=\"http://yanxuan.nosdn.127.net/2974fb17474f1e75a3746cbdb9d38d08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2aacbef9ae23bbda05115240a09711d2.jpg\" _src=\"http://yanxuan.nosdn.127.net/2aacbef9ae23bbda05115240a09711d2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b09d8a77f61eb9c0e2598f090a9903d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b09d8a77f61eb9c0e2598f090a9903d1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79277de533411ec1556af43c2214cd2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/79277de533411ec1556af43c2214cd2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5223bbdf9b7f3206ae48fc41d0f8870f.jpg\" _src=\"http://yanxuan.nosdn.127.net/5223bbdf9b7f3206ae48fc41d0f8870f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1bdede2a5332a7cf7cb988d216219c8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1bdede2a5332a7cf7cb988d216219c8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9bc8c2543a42a80d980d90bb49f761f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9bc8c2543a42a80d980d90bb49f761f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a6ac4fcd6367432ea61eb2c9b972c85b.jpg\" _src=\"http://yanxuan.nosdn.127.net/a6ac4fcd6367432ea61eb2c9b972c85b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8cf923bfea6642309dd45f23cc0db014.jpg\" _src=\"http://yanxuan.nosdn.127.net/8cf923bfea6642309dd45f23cc0db014.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/038854293eb327038bff7f9b12ecc959.jpg\" _src=\"http://yanxuan.nosdn.127.net/038854293eb327038bff7f9b12ecc959.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb39a24c1e3af6e98b04dadbd33a3fe9.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb39a24c1e3af6e98b04dadbd33a3fe9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/362b2f3046711bc23186648dae74ad6d.jpg\" _src=\"http://yanxuan.nosdn.127.net/362b2f3046711bc23186648dae74ad6d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/49f7de4e37e5ecd2f7164ede19d9f733.jpg\" _src=\"http://yanxuan.nosdn.127.net/49f7de4e37e5ecd2f7164ede19d9f733.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/569e9d6b44ca2f27a1c12509e8915e66.jpg\" _src=\"http://yanxuan.nosdn.127.net/569e9d6b44ca2f27a1c12509e8915e66.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c5dc22bfcd8a766721a4627e543ed910.jpg\" _src=\"http://yanxuan.nosdn.127.net/c5dc22bfcd8a766721a4627e543ed910.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/713237ccefdecfdc349a112cdf19dad4.jpg\" _src=\"http://yanxuan.nosdn.127.net/713237ccefdecfdc349a112cdf19dad4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/90fbeb1d0446c8478ff02401def15c2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/90fbeb1d0446c8478ff02401def15c2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5044c7429edbfbb7b839e557fd8f818d.jpg\" _src=\"http://yanxuan.nosdn.127.net/5044c7429edbfbb7b839e557fd8f818d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5aec8b5df3e773ee8b14113a2cdcb32.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5aec8b5df3e773ee8b14113a2cdcb32.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfd9bccd47e871bc7f67779bc784db51.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfd9bccd47e871bc7f67779bc784db51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ffa489f82e9d2aa77393cd7f65ebee86.jpg\" _src=\"http://yanxuan.nosdn.127.net/ffa489f82e9d2aa77393cd7f65ebee86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd56dc555af6f50272e7cd31e29644c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd56dc555af6f50272e7cd31e29644c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d261318f912c3b09ae24c7efdb55647.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d261318f912c3b09ae24c7efdb55647.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1cf1335f9646f9e3b82ad4b21540f0b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/1cf1335f9646f9e3b82ad4b21540f0b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9881c742b4178a4096b2faf8630fdf48.jpg\" _src=\"http://yanxuan.nosdn.127.net/9881c742b4178a4096b2faf8630fdf48.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e1fb2de40eb0243aa204ea419534d9c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e1fb2de40eb0243aa204ea419534d9c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c4699bbb0bb64091ea65c2fcb48571f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/c4699bbb0bb64091ea65c2fcb48571f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31bbf71652f62fa75caaa1c17619046e.jpg\" _src=\"http://yanxuan.nosdn.127.net/31bbf71652f62fa75caaa1c17619046e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2784a49f991209e108573e1576c737db.jpg\" _src=\"http://yanxuan.nosdn.127.net/2784a49f991209e108573e1576c737db.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/032f984b95d0557c42b381c5dac63bba.jpg\" _src=\"http://yanxuan.nosdn.127.net/032f984b95d0557c42b381c5dac63bba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/649c19a764f92a7f7caa2901e91fced7.jpg\" _src=\"http://yanxuan.nosdn.127.net/649c19a764f92a7f7caa2901e91fced7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ce2a4df0ccb346bc78507d033ed41ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ce2a4df0ccb346bc78507d033ed41ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c304880b8d2184655ad0f2fa9cb80663.jpg\" _src=\"http://yanxuan.nosdn.127.net/c304880b8d2184655ad0f2fa9cb80663.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c6e5ff7cdff06f1489816156c75c6dd6.jpg\" _src=\"http://yanxuan.nosdn.127.net/c6e5ff7cdff06f1489816156c75c6dd6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/542c796e0f10192cc950bddb418b6953.jpg\" _src=\"http://yanxuan.nosdn.127.net/542c796e0f10192cc950bddb418b6953.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/675bd2b57d02e966da0981017acc9ffc.jpg\" _src=\"http://yanxuan.nosdn.127.net/675bd2b57d02e966da0981017acc9ffc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ec3a06d23be8c6ea4bad1ab55394af2.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ec3a06d23be8c6ea4bad1ab55394af2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59434b29c18dff0207a6560970335a0b.jpg\" _src=\"http://yanxuan.nosdn.127.net/59434b29c18dff0207a6560970335a0b.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 4,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/19e7760c63ae6dc154a078460d183542.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/deeb55bb45f94cb236a47d1264e883b8.png",
      "retail_price": 299,
      "sell_volume": 5402,
      "primary_product_id": 1111049,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1115028,
      "category_id": 1008009,
      "goods_sn": "1115028",
      "name": "日式色织水洗棉条纹四件套",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "纯棉水洗感，柔软吸汗",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/c7a4904d00fec84dcb8d024acf9c9124.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7a4904d00fec84dcb8d024acf9c9124.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ca8260a0e668703f99b76d2b5febe39.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ca8260a0e668703f99b76d2b5febe39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a8001ac179af2b6a9710754ab3be0a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a8001ac179af2b6a9710754ab3be0a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4565564e3359df7c1bfa3ad75d482fff.jpg\" _src=\"http://yanxuan.nosdn.127.net/4565564e3359df7c1bfa3ad75d482fff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd7ace2c6a2c4324ef5e1f9355e89268.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd7ace2c6a2c4324ef5e1f9355e89268.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb9241fa90a48c6f9820785c728d2bff.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb9241fa90a48c6f9820785c728d2bff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8fae72fff469beacc683209a4514a41f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8fae72fff469beacc683209a4514a41f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/395d99acde8e480bde8dc765ac1eb580.jpg\" _src=\"http://yanxuan.nosdn.127.net/395d99acde8e480bde8dc765ac1eb580.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f5a5bc28c4db2fffc72228668a09534.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f5a5bc28c4db2fffc72228668a09534.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/849c44ecb9149dbe4186fd2a7176c2b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/849c44ecb9149dbe4186fd2a7176c2b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85c02b7f73716798a07078ca99a84dcc.jpg\" _src=\"http://yanxuan.nosdn.127.net/85c02b7f73716798a07078ca99a84dcc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02e8ed22c5110a71db1bbe3ea911246d.jpg\" _src=\"http://yanxuan.nosdn.127.net/02e8ed22c5110a71db1bbe3ea911246d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d668a817a0c0fbf2c550fb2732e3278.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d668a817a0c0fbf2c550fb2732e3278.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7504ed0982387d5837de6f146aeae2a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/7504ed0982387d5837de6f146aeae2a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5825013e93079cd9389a1a85db9ea986.jpg\" _src=\"http://yanxuan.nosdn.127.net/5825013e93079cd9389a1a85db9ea986.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c9895d59d2ce2c2f05b7d7d342edf8b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c9895d59d2ce2c2f05b7d7d342edf8b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85c29c4c8fb2db231665bcbf2322671d.jpg\" _src=\"http://yanxuan.nosdn.127.net/85c29c4c8fb2db231665bcbf2322671d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/57615e82ddcb6f5b4eb1239d3948d8fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/57615e82ddcb6f5b4eb1239d3948d8fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/518b4a422d10e1075a76bb79232391e6.jpg\" _src=\"http://yanxuan.nosdn.127.net/518b4a422d10e1075a76bb79232391e6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d5928965b398160fdfef1a1a826bac75.jpg\" _src=\"http://yanxuan.nosdn.127.net/d5928965b398160fdfef1a1a826bac75.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6271c3f5120f19b42bb913e6945cbf95.jpg\" _src=\"http://yanxuan.nosdn.127.net/6271c3f5120f19b42bb913e6945cbf95.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/674aee6d3a58fb51551f6766689bc7ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/674aee6d3a58fb51551f6766689bc7ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29f78e78e62742cff9b760a9b97e4347.jpg\" _src=\"http://yanxuan.nosdn.127.net/29f78e78e62742cff9b760a9b97e4347.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/755ac0784730b54dc44fc2a3fc97d941.jpg\" _src=\"http://yanxuan.nosdn.127.net/755ac0784730b54dc44fc2a3fc97d941.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b0cd4cc9a627be11362be64fa4bcbf06.jpg\" _src=\"http://yanxuan.nosdn.127.net/b0cd4cc9a627be11362be64fa4bcbf06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3205cd14570da7022b1943da198763f0.jpg\" _src=\"http://yanxuan.nosdn.127.net/3205cd14570da7022b1943da198763f0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f263b42fc5808f4de777410befd094cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/f263b42fc5808f4de777410befd094cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93d0a8bea9bd2f52941628dff09ef381.jpg\" _src=\"http://yanxuan.nosdn.127.net/93d0a8bea9bd2f52941628dff09ef381.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97e43d6548d7215956380ffd0c5a1810.jpg\" _src=\"http://yanxuan.nosdn.127.net/97e43d6548d7215956380ffd0c5a1810.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e3e8b023e2dbf472c8889456c00cf9be.jpg\" _src=\"http://yanxuan.nosdn.127.net/e3e8b023e2dbf472c8889456c00cf9be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/158be4bab49629d527bd8e27e55c77d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/158be4bab49629d527bd8e27e55c77d1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d345c8615953a60a424e5a47c0cd16a.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d345c8615953a60a424e5a47c0cd16a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff89423e056191c2d4a12196b900d7f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff89423e056191c2d4a12196b900d7f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e953286fce6c89f74ce7150f2f478d64.jpg\" _src=\"http://yanxuan.nosdn.127.net/e953286fce6c89f74ce7150f2f478d64.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff0d95c718fe73cd66dff1de8a43d7a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff0d95c718fe73cd66dff1de8a43d7a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c2009a46185b6bd5463528971ef2c2af.jpg\" _src=\"http://yanxuan.nosdn.127.net/c2009a46185b6bd5463528971ef2c2af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f08bae55ef68af811f57ff105ec5ec3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/f08bae55ef68af811f57ff105ec5ec3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84ac737dabdb85482f2ce39df119c753.jpg\" _src=\"http://yanxuan.nosdn.127.net/84ac737dabdb85482f2ce39df119c753.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fc95259418359a519d7f604af79d6f19.jpg\" _src=\"http://yanxuan.nosdn.127.net/fc95259418359a519d7f604af79d6f19.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b673c4829dceec9488b5bddacc3ae7c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b673c4829dceec9488b5bddacc3ae7c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da72e531c1bc3bba73d61456396dcaba.jpg\" _src=\"http://yanxuan.nosdn.127.net/da72e531c1bc3bba73d61456396dcaba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10e489150f5b12c3fed27560df0cb391.jpg\" _src=\"http://yanxuan.nosdn.127.net/10e489150f5b12c3fed27560df0cb391.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fc42020bc2b630c1be212b734bf70e53.jpg\" _src=\"http://yanxuan.nosdn.127.net/fc42020bc2b630c1be212b734bf70e53.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f27be3e26b925f26d81e5f90b12cd1cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/f27be3e26b925f26d81e5f90b12cd1cf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33e9cfb394b44658be3ab3fbae977638.jpg\" _src=\"http://yanxuan.nosdn.127.net/33e9cfb394b44658be3ab3fbae977638.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/008e03c492bf5b1cf9a3b94c525e3920.jpg\" _src=\"http://yanxuan.nosdn.127.net/008e03c492bf5b1cf9a3b94c525e3920.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e4bc8cbbb6b937bb0b122649a4560e1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/e4bc8cbbb6b937bb0b122649a4560e1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbee4d90772a3e0c40811de3fd2cfdea.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbee4d90772a3e0c40811de3fd2cfdea.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 5,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/34ce3734403b04de2a027206237aad6f.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/3d0045e8f43439c7004fae052b2162ed.png",
      "retail_price": 299,
      "sell_volume": 4440,
      "primary_product_id": 1116061,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1130037,
      "category_id": 1008002,
      "goods_sn": "1130037",
      "name": "帆布丝羽绒多用坐垫",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "柔软蓬松，透气防螨。",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/96eb609f4f459ab9c502eca7d6e7e204.jpg\" _src=\"http://yanxuan.nosdn.127.net/96eb609f4f459ab9c502eca7d6e7e204.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a86dcf95f3a56db6b7f99f35585dbf2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a86dcf95f3a56db6b7f99f35585dbf2d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bced9d39bcb740a4655ce725f4823e96.jpg\" _src=\"http://yanxuan.nosdn.127.net/bced9d39bcb740a4655ce725f4823e96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11213e448a23292458adc934a643c076.jpg\" _src=\"http://yanxuan.nosdn.127.net/11213e448a23292458adc934a643c076.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9116d858fd59f1ed32fc8a692dfc3fed.jpg\" _src=\"http://yanxuan.nosdn.127.net/9116d858fd59f1ed32fc8a692dfc3fed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b5982e9a43ccaa724f397c9e777b026.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b5982e9a43ccaa724f397c9e777b026.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e4397bee1cf9589eaaf06b8fe9d0a778.jpg\" _src=\"http://yanxuan.nosdn.127.net/e4397bee1cf9589eaaf06b8fe9d0a778.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/740affd3cef0ef40378c2cb265322f15.jpg\" _src=\"http://yanxuan.nosdn.127.net/740affd3cef0ef40378c2cb265322f15.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6aeacc205ef12e2a475eb7a8e8d1eedc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6aeacc205ef12e2a475eb7a8e8d1eedc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/119709a17d08f2c1c48d95d24b34ca3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/119709a17d08f2c1c48d95d24b34ca3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8332210d4b81d04f42612fc097db259a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8332210d4b81d04f42612fc097db259a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be1775926acb0e26b6012cba7893e979.jpg\" _src=\"http://yanxuan.nosdn.127.net/be1775926acb0e26b6012cba7893e979.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c6463b2f53c89273f1f79b22dd9e399.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c6463b2f53c89273f1f79b22dd9e399.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38ad3258ebf23df5164854fe403d1ecf.jpg\" _src=\"http://yanxuan.nosdn.127.net/38ad3258ebf23df5164854fe403d1ecf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dc5f238dcb73c249f813233d81156c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dc5f238dcb73c249f813233d81156c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb132e2e8a254b8cbc345900f6fe3c39.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb132e2e8a254b8cbc345900f6fe3c39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0603f40fefd14ee24e83102c5f09100a.jpg\" _src=\"http://yanxuan.nosdn.127.net/0603f40fefd14ee24e83102c5f09100a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/45966f38135adc1280a667040d8e02c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/45966f38135adc1280a667040d8e02c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1064a54404b6c795eae261334697e050.jpg\" _src=\"http://yanxuan.nosdn.127.net/1064a54404b6c795eae261334697e050.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ef89417a81ac1893c95179585bf1140.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ef89417a81ac1893c95179585bf1140.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c2cd2da4d75a63ada7c655e53c223a0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/c2cd2da4d75a63ada7c655e53c223a0e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e942519448a5de394885730e0e3e4694.jpg\" _src=\"http://yanxuan.nosdn.127.net/e942519448a5de394885730e0e3e4694.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d016a18c381916813c2eaf46c3f791c1.jpg\" _src=\"http://yanxuan.nosdn.127.net/d016a18c381916813c2eaf46c3f791c1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6935f94bc80c11c89c3f8a2aa02c4273.jpg\" _src=\"http://yanxuan.nosdn.127.net/6935f94bc80c11c89c3f8a2aa02c4273.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9dedb80199b09770b98fa46cd8a8752d.jpg\" _src=\"http://yanxuan.nosdn.127.net/9dedb80199b09770b98fa46cd8a8752d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f447537304e43a44b1e75272d3334899.jpg\" _src=\"http://yanxuan.nosdn.127.net/f447537304e43a44b1e75272d3334899.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10d901511a3d5f03be68bd64dbadfe1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/10d901511a3d5f03be68bd64dbadfe1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b03a90f7bb697a9bc6e0be9d9997b11.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b03a90f7bb697a9bc6e0be9d9997b11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62b277f50e7cca075cd2565a4f2b4466.jpg\" _src=\"http://yanxuan.nosdn.127.net/62b277f50e7cca075cd2565a4f2b4466.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e304f8f1ea10792be9072d3c7a4a8359.jpg\" _src=\"http://yanxuan.nosdn.127.net/e304f8f1ea10792be9072d3c7a4a8359.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d7c39350bee7fdc8bdb78a27eb83a17.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d7c39350bee7fdc8bdb78a27eb83a17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/742927f31cadc641a7b9bb3fc5eebfe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/742927f31cadc641a7b9bb3fc5eebfe3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2562d7d1a0fa4b9497e4ec719f08a8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2562d7d1a0fa4b9497e4ec719f08a8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/430442f4524e66347fbbf10aaf213a07.jpg\" _src=\"http://yanxuan.nosdn.127.net/430442f4524e66347fbbf10aaf213a07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/620ec1f6387fa84f5518ad2484ebaa91.jpg\" _src=\"http://yanxuan.nosdn.127.net/620ec1f6387fa84f5518ad2484ebaa91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/455f215b9a402ed9c0c0972c0abddbb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/455f215b9a402ed9c0c0972c0abddbb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1def5c3403bdf5cd7e11b85354542452.jpg\" _src=\"http://yanxuan.nosdn.127.net/1def5c3403bdf5cd7e11b85354542452.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97348238ae3c27a56ff46e1b6c3deb3b.jpg\" _src=\"http://yanxuan.nosdn.127.net/97348238ae3c27a56ff46e1b6c3deb3b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3739461a5eb338a70e7d34a86ff26d1a.jpg\" _src=\"http://yanxuan.nosdn.127.net/3739461a5eb338a70e7d34a86ff26d1a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/96fae2f2cc374d459c3969e7a7cc1a83.jpg\" _src=\"http://yanxuan.nosdn.127.net/96fae2f2cc374d459c3969e7a7cc1a83.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c1654fc509c8c77e9fe4c75ffc099f24.jpg\" _src=\"http://yanxuan.nosdn.127.net/c1654fc509c8c77e9fe4c75ffc099f24.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf95ab8945e61c7180eba1e01721b15a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf95ab8945e61c7180eba1e01721b15a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b054e088382a0cb32a529082c52745e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b054e088382a0cb32a529082c52745e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d517d1ca7532cde5cc74ad2a10dc17.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d517d1ca7532cde5cc74ad2a10dc17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6222e1fd9b42422e8454cc087a0e0358.jpg\" _src=\"http://yanxuan.nosdn.127.net/6222e1fd9b42422e8454cc087a0e0358.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8995022af1826e846b7a143e7b8b325.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8995022af1826e846b7a143e7b8b325.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a12c940956234db2f60a2b5b51d6a35.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a12c940956234db2f60a2b5b51d6a35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4be7d3058e6eec27a4be033642359535.jpg\" _src=\"http://yanxuan.nosdn.127.net/4be7d3058e6eec27a4be033642359535.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2eca2f02d4ec269cc1893876fb17511a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2eca2f02d4ec269cc1893876fb17511a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf761716e3b430f63e059a891703200e.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf761716e3b430f63e059a891703200e.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 17,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2d1f51656c0bff4989e43b17b42f7ad9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/19ecd7c6f6f31219cf75117238d95139.png",
      "retail_price": 39,
      "sell_volume": 9661,
      "primary_product_id": 1130120,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    }
  ]
}
```

### 商品分类列表

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/category/indexaction `

**请求方式：**

- GET 

**返回示例**

```json
{
  "categoryList": [
    {
      "id": 1005000,
      "name": "居家",
      "keywords": "",
      "front_desc": "回家，放松身心",
      "parent_id": 0,
      "sort_order": 2,
      "show_index": 1,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/92357337378cce650797444bc107b0f7.jpg",
      "icon_url": "http://yanxuan.nosdn.127.net/a45c2c262a476fea0b9fc684fed91ef5.png",
      "img_url": "//nos.netease.com/yanxuan/f0d0e1a542e2095861b42bf789d948ce.jpg",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/e8bf0cf08cf7eda21606ab191762e35c.png",
      "level": "L1",
      "type": 0,
      "front_name": "回家，放松身心"
    },
    {
      "id": 1005001,
      "name": "餐厨",
      "keywords": "",
      "front_desc": "厨房",
      "parent_id": 0,
      "sort_order": 3,
      "show_index": 2,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/f4ff8b3d5b0767d4e578575c1fd6b921.jpg",
      "icon_url": "http://yanxuan.nosdn.127.net/ad8b00d084cb7d0958998edb5fee9c0a.png",
      "img_url": "//nos.netease.com/yanxuan/88855173a0cfcfd889ee6394a3259c4f.jpg",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/3708dbcb35ad5abf9e001500f73db615.png",
      "level": "L1",
      "type": 0,
      "front_name": "爱，囿于厨房"
  ]
}
```

### 商品分类子分类

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/category/currentaction `

**请求方式：**

- GET 

**参数：** 

| 参数名 | 必选  | 类型  | 说明  |
|:--- |:--- |:--- | --- |
| id  | 是   | int | 无   |

**返回示例**

```json
{
  "data": {
    "currentOne": {
      "id": 1005000,
      "name": "居家",
      "keywords": "",
      "front_desc": "回家，放松身心",
      "parent_id": 0,
      "sort_order": 2,
      "show_index": 1,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/92357337378cce650797444bc107b0f7.jpg",
      "icon_url": "http://yanxuan.nosdn.127.net/a45c2c262a476fea0b9fc684fed91ef5.png",
      "img_url": "//nos.netease.com/yanxuan/f0d0e1a542e2095861b42bf789d948ce.jpg",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/e8bf0cf08cf7eda21606ab191762e35c.png",
      "level": "L1",
      "type": 0,
      "front_name": "回家，放松身心",
      "subList": [
        {
          "id": 1008002,
          "name": "布艺软装",
          "keywords": "",
          "front_desc": "换个软装，换个家",
          "parent_id": 1005000,
          "sort_order": 6,
          "show_index": 4,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/8bbcd7de60a678846664af998f57e71c.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/2e2fb4f2856a021bbcd1b4c8400f2b06.png",
          "level": "L2",
          "type": 0,
          "front_name": "各种风格软装装点你的家"
        },
        {
          "id": 1008008,
          "name": "被枕",
          "keywords": "",
          "front_desc": "选用优质材料，确保好芯",
          "parent_id": 1005000,
          "sort_order": 2,
          "show_index": 2,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/927bc33f7ae2895dd6c11cf91f5e3228.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/b43ef7cececebe6292d2f7f590522e05.png",
          "level": "L2",
          "type": 0,
          "front_name": "守护你的睡眠时光"
        },
        {
          "id": 1008009,
          "name": "床品件套",
          "keywords": "",
          "front_desc": "严格用料，亲肤舒适",
          "parent_id": 1005000,
          "sort_order": 4,
          "show_index": 3,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/243e5bf327a87217ad1f54592f0176ec.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/81f671bd36bce05d5f57827e5c88dd1b.png",
          "level": "L2",
          "type": 0,
          "front_name": "MUJI等品牌制造商出品"
        },
        {
          "id": 1008016,
          "name": "灯具",
          "keywords": "",
          "front_desc": "极简主义，贴近生活的设计",
          "parent_id": 1005000,
          "sort_order": 8,
          "show_index": 6,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/c48e0d9dcfac01499a437774a915842b.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/f702dc399d14d4e1509d5ed6e57acd19.png",
          "level": "L2",
          "type": 0,
          "front_name": "一盏灯，温暖一个家"
        },
        {
          "id": 1010003,
          "name": "地垫",
          "keywords": "",
          "front_desc": "手工编织，时尚环保",
          "parent_id": 1005000,
          "sort_order": 5,
          "show_index": 4,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/83d4c87f28c993af1aa8d3e4d30a2fa2.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/1611ef6458e244d1909218becfe87c4d.png",
          "level": "L2",
          "type": 0,
          "front_name": "家里的第“五”面墙"
        },
        {
          "id": 1011003,
          "name": "床垫",
          "keywords": "",
          "front_desc": "助你拥有舒眠好梦",
          "parent_id": 1005000,
          "sort_order": 3,
          "show_index": 3,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/316afeb3948b295dfe073e4c51f77a42.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/d6e0e84961032fc70fd52a8d4d0fb514.png",
          "level": "L2",
          "type": 0,
          "front_name": "承托你的好时光"
        },
        {
          "id": 1011004,
          "name": "家饰",
          "keywords": "",
          "front_desc": "点缀美好生活，品质在于细节",
          "parent_id": 1005000,
          "sort_order": 9,
          "show_index": 7,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/ab0df9445d985bf6719ac415313a8e88.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/79275db76b5865e6167b0fbd141f2d7e.png",
          "level": "L2",
          "type": 0,
          "front_name": "装饰你的家"
        },
        {
          "id": 1015000,
          "name": "家具",
          "keywords": "",
          "front_desc": "一级原木，严苛工艺",
          "parent_id": 1005000,
          "sort_order": 7,
          "show_index": 5,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/4f00675caefd0d4177892ad18bfc2df6.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/d5d41841136182bf49c1f99f5c452dd6.png",
          "level": "L2",
          "type": 0,
          "front_name": "大师级工艺"
        },
        {
          "id": 1017000,
          "name": "宠物",
          "keywords": "",
          "front_desc": "出口品质，严选贴合萌宠生活习惯用品。",
          "parent_id": 1005000,
          "sort_order": 10,
          "show_index": 8,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/a0352c57c60ce4f68370ecdab6a30857.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/dae4d6e89ab8a0cd3e8da026e4660137.png",
          "level": "L2",
          "type": 0,
          "front_name": "抑菌除味，打造宠物舒适空间"
        },
        {
          "id": 1036000,
          "name": "夏凉",
          "keywords": "",
          "front_desc": "夏凉床品，舒适一夏",
          "parent_id": 1005000,
          "sort_order": 1,
          "show_index": 1,
          "is_show": 1,
          "banner_url": "http://yanxuan.nosdn.127.net/13ff4decdf38fe1a5bde34f0e0cc635a.png",
          "icon_url": "",
          "img_url": "",
          "wap_banner_url": "http://yanxuan.nosdn.127.net/bd17c985bacb9b9ab1ab6e9d66ee343c.png",
          "level": "L2",
          "type": 0,
          "front_name": "夏凉床品，舒适一夏"

      ]
    }
  }
}
```

### 商品子分类导航

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/category/categoryNav `

**请求方式：**

- GET 

**参数：** 

| 参数名 | 必选  | 类型  | 说明    |
|:--- |:--- |:--- | ----- |
| id  | 是   | int | 子分类id |

**返回示例**

```json
{
  "navData": [
    {
      "id": 1008002,
      "name": "布艺软装",
      "keywords": "",
      "front_desc": "换个软装，换个家",
      "parent_id": 1005000,
      "sort_order": 6,
      "show_index": 4,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/8bbcd7de60a678846664af998f57e71c.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/2e2fb4f2856a021bbcd1b4c8400f2b06.png",
      "level": "L2",
      "type": 0,
      "front_name": "各种风格软装装点你的家"
    },
    {
      "id": 1008008,
      "name": "被枕",
      "keywords": "",
      "front_desc": "选用优质材料，确保好芯",
      "parent_id": 1005000,
      "sort_order": 2,
      "show_index": 2,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/927bc33f7ae2895dd6c11cf91f5e3228.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/b43ef7cececebe6292d2f7f590522e05.png",
      "level": "L2",
      "type": 0,
      "front_name": "守护你的睡眠时光"
    },
    {
      "id": 1008009,
      "name": "床品件套",
      "keywords": "",
      "front_desc": "严格用料，亲肤舒适",
      "parent_id": 1005000,
      "sort_order": 4,
      "show_index": 3,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/243e5bf327a87217ad1f54592f0176ec.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/81f671bd36bce05d5f57827e5c88dd1b.png",
      "level": "L2",
      "type": 0,
      "front_name": "MUJI等品牌制造商出品"
    },
    {
      "id": 1008016,
      "name": "灯具",
      "keywords": "",
      "front_desc": "极简主义，贴近生活的设计",
      "parent_id": 1005000,
      "sort_order": 8,
      "show_index": 6,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/c48e0d9dcfac01499a437774a915842b.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/f702dc399d14d4e1509d5ed6e57acd19.png",
      "level": "L2",
      "type": 0,
      "front_name": "一盏灯，温暖一个家"
    },
    {
      "id": 1010003,
      "name": "地垫",
      "keywords": "",
      "front_desc": "手工编织，时尚环保",
      "parent_id": 1005000,
      "sort_order": 5,
      "show_index": 4,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/83d4c87f28c993af1aa8d3e4d30a2fa2.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/1611ef6458e244d1909218becfe87c4d.png",
      "level": "L2",
      "type": 0,
      "front_name": "家里的第“五”面墙"
    },
    {
      "id": 1011003,
      "name": "床垫",
      "keywords": "",
      "front_desc": "助你拥有舒眠好梦",
      "parent_id": 1005000,
      "sort_order": 3,
      "show_index": 3,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/316afeb3948b295dfe073e4c51f77a42.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/d6e0e84961032fc70fd52a8d4d0fb514.png",
      "level": "L2",
      "type": 0,
      "front_name": "承托你的好时光"
    },
    {
      "id": 1011004,
      "name": "家饰",
      "keywords": "",
      "front_desc": "点缀美好生活，品质在于细节",
      "parent_id": 1005000,
      "sort_order": 9,
      "show_index": 7,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/ab0df9445d985bf6719ac415313a8e88.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/79275db76b5865e6167b0fbd141f2d7e.png",
      "level": "L2",
      "type": 0,
      "front_name": "装饰你的家"
    },
    {
      "id": 1015000,
      "name": "家具",
      "keywords": "",
      "front_desc": "一级原木，严苛工艺",
      "parent_id": 1005000,
      "sort_order": 7,
      "show_index": 5,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/4f00675caefd0d4177892ad18bfc2df6.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/d5d41841136182bf49c1f99f5c452dd6.png",
      "level": "L2",
      "type": 0,
      "front_name": "大师级工艺"
    },
    {
      "id": 1017000,
      "name": "宠物",
      "keywords": "",
      "front_desc": "出口品质，严选贴合萌宠生活习惯用品。",
      "parent_id": 1005000,
      "sort_order": 10,
      "show_index": 8,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/a0352c57c60ce4f68370ecdab6a30857.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/dae4d6e89ab8a0cd3e8da026e4660137.png",
      "level": "L2",
      "type": 0,
      "front_name": "抑菌除味，打造宠物舒适空间"
    },
    {
      "id": 1036000,
      "name": "夏凉",
      "keywords": "",
      "front_desc": "夏凉床品，舒适一夏",
      "parent_id": 1005000,
      "sort_order": 1,
      "show_index": 1,
      "is_show": 1,
      "banner_url": "http://yanxuan.nosdn.127.net/13ff4decdf38fe1a5bde34f0e0cc635a.png",
      "icon_url": "",
      "img_url": "",
      "wap_banner_url": "http://yanxuan.nosdn.127.net/bd17c985bacb9b9ab1ab6e9d66ee343c.png",
      "level": "L2",
      "type": 0,
      "front_name": "夏凉床品，舒适一夏"
    }
  ],
  "currentNav": {
    "id": 1008008,
    "name": "被枕",
    "keywords": "",
    "front_desc": "选用优质材料，确保好芯",
    "parent_id": 1005000,
    "sort_order": 2,
    "show_index": 2,
    "is_show": 1,
    "banner_url": "http://yanxuan.nosdn.127.net/927bc33f7ae2895dd6c11cf91f5e3228.png",
    "icon_url": "",
    "img_url": "",
    "wap_banner_url": "http://yanxuan.nosdn.127.net/b43ef7cececebe6292d2f7f590522e05.png",
    "level": "L2",
    "type": 0,
    "front_name": "守护你的睡眠时光"
  }
}
```

### 获取分类商品列表

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/goods/goodsList `

**请求方式：**

- GET 

**参数：** 

| 参数名        | 必选  | 类型  | 说明   |
|:---------- |:--- |:--- | ---- |
| categoryId | 是   | int | 分类id |

**返回示例**

```json
{
  "data": [
    {
      "id": 1009024,
      "category_id": 1008002,
      "goods_sn": "1009024",
      "name": "日式和风懒人沙发",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "优质莱卡纯棉，和风家居新体验",
      "goods_desc": "<p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/34a6a0daa3f7a397a38aad14cb9e90fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/34a6a0daa3f7a397a38aad14cb9e90fa.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/76637af0eec246b318cb129b768de637.jpg\" _src=\"http://yanxuan.nosdn.127.net/76637af0eec246b318cb129b768de637.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18fee22626e61fc1d1a01916914016ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/18fee22626e61fc1d1a01916914016ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91f57a9bb142e1c1e2ff0bbea6f9af96.jpg\" _src=\"http://yanxuan.nosdn.127.net/91f57a9bb142e1c1e2ff0bbea6f9af96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/252d80fd75eb1254d746d0b57c267650.jpg\" _src=\"http://yanxuan.nosdn.127.net/252d80fd75eb1254d746d0b57c267650.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b07697992a2b14de6fd0a5811936d71.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b07697992a2b14de6fd0a5811936d71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c499439d6081bb4e836955b7514c1b96.jpg\" _src=\"http://yanxuan.nosdn.127.net/c499439d6081bb4e836955b7514c1b96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bed437fdc091d020a8f805bcc8830bd8.jpg\" _src=\"http://yanxuan.nosdn.127.net/bed437fdc091d020a8f805bcc8830bd8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fc5febdb817abd7a1040bab03f048b7.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fc5febdb817abd7a1040bab03f048b7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a0417b3986c9dc082124fcc360390021.jpg\" _src=\"http://yanxuan.nosdn.127.net/a0417b3986c9dc082124fcc360390021.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a5c9d24c652d4dee7946ef925105f3f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/a5c9d24c652d4dee7946ef925105f3f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b10272c58f95dd6737ce1cd41452a21d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b10272c58f95dd6737ce1cd41452a21d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/510c6ef36760238b38ed59cd6e47a21f.png\" _src=\"http://yanxuan.nosdn.127.net/510c6ef36760238b38ed59cd6e47a21f.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6371348b917c021c55dc393fc59d4d28.png\" _src=\"http://yanxuan.nosdn.127.net/6371348b917c021c55dc393fc59d4d28.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de4079b128e57c5c0fa8a8177e9bc6e7.png\" _src=\"http://yanxuan.nosdn.127.net/de4079b128e57c5c0fa8a8177e9bc6e7.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/160966fbc772787f824dc1dbd5afb16d.png\" _src=\"http://yanxuan.nosdn.127.net/160966fbc772787f824dc1dbd5afb16d.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb3c8d3f10f2aca0908871c8e598aa0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb3c8d3f10f2aca0908871c8e598aa0e.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 1,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/bcaf7ee314af7dbfb04612087e563249.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/149dfa87a7324e184c5526ead81de9ad.png",
      "retail_price": 599,
      "sell_volume": 2918,
      "primary_product_id": 1008052,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1015007,
      "category_id": 1008002,
      "goods_sn": "1015007",
      "name": "典雅美式全棉刺绣抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "典雅毛线绣，精致工艺",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/66640f55aeb668ac9df6e26b6b30adb5.jpg\" _src=\"http://yanxuan.nosdn.127.net/66640f55aeb668ac9df6e26b6b30adb5.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/42852faba5623c6dc5be451d80e5df03.jpg\" _src=\"http://yanxuan.nosdn.127.net/42852faba5623c6dc5be451d80e5df03.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48ce93c6f6a731778c505442f163b09e.jpg\" _src=\"http://yanxuan.nosdn.127.net/48ce93c6f6a731778c505442f163b09e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02a3abee9bb3e22f27781ced8774d1ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/02a3abee9bb3e22f27781ced8774d1ab.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c62a27145e1045879e3f2b97b9f86b4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/c62a27145e1045879e3f2b97b9f86b4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48baaafe4ea4c32242c57e58ce8e139f.jpg\" _src=\"http://yanxuan.nosdn.127.net/48baaafe4ea4c32242c57e58ce8e139f.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99549f0375b108240866a09a0a2527d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/99549f0375b108240866a09a0a2527d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/341529ba80d91c5304680be8f524a626.jpg\" _src=\"http://yanxuan.nosdn.127.net/341529ba80d91c5304680be8f524a626.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b15e35e9d8c04288dfb7546b1f743c17.jpg\" _src=\"http://yanxuan.nosdn.127.net/b15e35e9d8c04288dfb7546b1f743c17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c0ebf7949133cb382b6bf18c8a5a1c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c0ebf7949133cb382b6bf18c8a5a1c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfd25d0fa6dc13a335877360e3dab8d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfd25d0fa6dc13a335877360e3dab8d1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbcc420cef18e4a43589198ebfcc4fd1.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbcc420cef18e4a43589198ebfcc4fd1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15aa3e3ed45714d29ca062499db930ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/15aa3e3ed45714d29ca062499db930ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab6963b4e529810577f3e428c9d10af6.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab6963b4e529810577f3e428c9d10af6.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 4,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/d16d6fb25f3d6d8c356fcd8e178bdd26.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/a2045004de8a6225289376ad54317fc8.png",
      "retail_price": 59,
      "sell_volume": 133,
      "primary_product_id": 1013024,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1020000,
      "category_id": 1008002,
      "goods_sn": "1020000",
      "name": "升级款记忆绵护椎腰靠",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "人体工学设计，缓解腰背疼痛",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/8176934e414ec6c85078cb64322fe336.jpg\" _src=\"http://yanxuan.nosdn.127.net/8176934e414ec6c85078cb64322fe336.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33ff256b2f69de517f567ebb993dd08e.jpg\" _src=\"http://yanxuan.nosdn.127.net/33ff256b2f69de517f567ebb993dd08e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5204e4f7c7fa00866e270a93ec85a596.jpg\" _src=\"http://yanxuan.nosdn.127.net/5204e4f7c7fa00866e270a93ec85a596.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f3aed0164b92344f17ffbc0b8fc7ade.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f3aed0164b92344f17ffbc0b8fc7ade.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d2d94d8f0f10f17183954b69d09e2bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d2d94d8f0f10f17183954b69d09e2bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3921600dd00e2c49a7414035111b767d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3921600dd00e2c49a7414035111b767d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aef3c726fec0be6ce17089e06e753d4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/aef3c726fec0be6ce17089e06e753d4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/446fbad756b6327898cee40e7b67a0b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/446fbad756b6327898cee40e7b67a0b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0950b4fa1cac49eece29af35c6e69e4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/0950b4fa1cac49eece29af35c6e69e4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf7e88b2b57641ab81bbf36351db5ff8.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf7e88b2b57641ab81bbf36351db5ff8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d66b4714682aaff4ab082980a44b46.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d66b4714682aaff4ab082980a44b46.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7f2d82d7a5622dd9f6b0d44faed9fda.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7f2d82d7a5622dd9f6b0d44faed9fda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7fdc566d101b7cf73cee32f55b0f945.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7fdc566d101b7cf73cee32f55b0f945.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e04202364d1a0a1dc1a2a1ea871e45e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e04202364d1a0a1dc1a2a1ea871e45e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b3135ad6c01a2675fc7e96f6643ff7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b3135ad6c01a2675fc7e96f6643ff7f.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 15,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/84563d90b0c10c4d4a8229fd34cb4063.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/819fdf1f635a694166bcfdd426416e8c.png",
      "retail_price": 79,
      "sell_volume": 8586,
      "primary_product_id": 1018000,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1030001,
      "category_id": 1008002,
      "goods_sn": "1030001",
      "name": "160*230羊毛手工地毯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "印度进口，手工编织，简约百搭",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/fbe953060dd4282539ee78e22f9c326c.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbe953060dd4282539ee78e22f9c326c.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb6320b1b19fe349fca98dcb509ccb41.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb6320b1b19fe349fca98dcb509ccb41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e3517025dc8da160277d7c80c55a83f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e3517025dc8da160277d7c80c55a83f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c6d902b098a5009871e7dd2fc47d4aae.jpg\" _src=\"http://yanxuan.nosdn.127.net/c6d902b098a5009871e7dd2fc47d4aae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15b721ac1796a6a93c2925c45fbafa91.jpg\" _src=\"http://yanxuan.nosdn.127.net/15b721ac1796a6a93c2925c45fbafa91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c1e30ecc74b5b25869f892f51d4472b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c1e30ecc74b5b25869f892f51d4472b0.jpg\" style=\"\"/></p><p><br/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7ddc57f40d4ec7d7e1069fc24438e93.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7ddc57f40d4ec7d7e1069fc24438e93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/68e501bd5f6f2018ee275af62edcebce.jpg\" _src=\"http://yanxuan.nosdn.127.net/68e501bd5f6f2018ee275af62edcebce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6cd10a4cc89e2067421632172382410c.jpg\" _src=\"http://yanxuan.nosdn.127.net/6cd10a4cc89e2067421632172382410c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/81d9b02cc74f846bb29bfc57b4d8dab1.jpg\" _src=\"http://yanxuan.nosdn.127.net/81d9b02cc74f846bb29bfc57b4d8dab1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/30a9e77d7e0cab9b389bc4a7f4a0be13.jpg\" _src=\"http://yanxuan.nosdn.127.net/30a9e77d7e0cab9b389bc4a7f4a0be13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50513c57074971334c4b715d8b3cdfa1.jpg\" _src=\"http://yanxuan.nosdn.127.net/50513c57074971334c4b715d8b3cdfa1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5497b96a17e01db88d3b8999d78e111d.jpg\" _src=\"http://yanxuan.nosdn.127.net/5497b96a17e01db88d3b8999d78e111d.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3311094b3f6ac170477dbf31fdc36a43.jpg\" _src=\"http://yanxuan.nosdn.127.net/3311094b3f6ac170477dbf31fdc36a43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb7a1c7b6c6989af9c42a4e66de098e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb7a1c7b6c6989af9c42a4e66de098e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ac42cbdfaa06c00a1bbd22fd63308546.jpg\" _src=\"http://yanxuan.nosdn.127.net/ac42cbdfaa06c00a1bbd22fd63308546.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0d2bf9139a0ca351f0ae4cabece86277.jpg\" _src=\"http://yanxuan.nosdn.127.net/0d2bf9139a0ca351f0ae4cabece86277.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da1c0eef412d5ff9761a8659fa64d91b.jpg\" _src=\"http://yanxuan.nosdn.127.net/da1c0eef412d5ff9761a8659fa64d91b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba7017652cf73419da57393bb02ca6de.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba7017652cf73419da57393bb02ca6de.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 25,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/ca0d9199db70d7b7f2b9b2ea673c74a4.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/88dc5d80c6f84102f003ecd69c86e1cf.png",
      "retail_price": 969,
      "sell_volume": 657,
      "primary_product_id": 1029001,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1030002,
      "category_id": 1008002,
      "goods_sn": "1030002",
      "name": "160*230羊毛圈绒枪刺地毯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "印度进口，手工枪刺，简约百搭",
      "goods_desc": "<p><video id=\"tmpVedio0\" class=\"edui-upload-video video-js vjs-default-skin video-js\" controls=\"\" preload=\"auto\" width=\"100%\" height=\"\" data-setup=\"{}\"><source src=\"http://yanxuan.nosdn.127.net/4ca24b2fa0043eb7435d1ca24312b689.mp4\" type=\"video/mp4\"/></video>‍</p><p><img src=\"http://yanxuan.nosdn.127.net/4c409ac170dafe286e2cbd918b30a388.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c409ac170dafe286e2cbd918b30a388.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c4147de069c1c7d819711e683fae373.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c4147de069c1c7d819711e683fae373.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d4be2d9edd8481dfa51cc7b86a90b36.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d4be2d9edd8481dfa51cc7b86a90b36.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61be18dbb282646133551c2bc297fb36.jpg\" _src=\"http://yanxuan.nosdn.127.net/61be18dbb282646133551c2bc297fb36.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7160604c5bd97a0f1aef7f3a2a32b72b.jpg\" _src=\"http://yanxuan.nosdn.127.net/7160604c5bd97a0f1aef7f3a2a32b72b.jpg\" style=\"\"/></p><p><br/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/32c5969b18a85bc62d4a855c40ab6142.jpg\" _src=\"http://yanxuan.nosdn.127.net/32c5969b18a85bc62d4a855c40ab6142.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62189479f43fd283340ce0fad3706b00.jpg\" _src=\"http://yanxuan.nosdn.127.net/62189479f43fd283340ce0fad3706b00.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f39cb441e6778d5d39510099f8befd3a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f39cb441e6778d5d39510099f8befd3a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bbb06c48c23cdf11fd93f711512eed7.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bbb06c48c23cdf11fd93f711512eed7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c0701aef423ba84cb1aabe8d6a1ab8d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/c0701aef423ba84cb1aabe8d6a1ab8d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4dec1e3bf4d5812d7d9fbddf50657e73.jpg\" _src=\"http://yanxuan.nosdn.127.net/4dec1e3bf4d5812d7d9fbddf50657e73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44497f9ad25cb6d208cc564016c8fd54.jpg\" _src=\"http://yanxuan.nosdn.127.net/44497f9ad25cb6d208cc564016c8fd54.jpg\"/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/37de0870b61ed6e880936d22000c2e85.jpg\" _src=\"http://yanxuan.nosdn.127.net/37de0870b61ed6e880936d22000c2e85.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97906141bd8846ea9e7888fa8a6b4ae0.jpg\" _src=\"http://yanxuan.nosdn.127.net/97906141bd8846ea9e7888fa8a6b4ae0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db23e00419f012686aaf4b3eeecae09b.jpg\" _src=\"http://yanxuan.nosdn.127.net/db23e00419f012686aaf4b3eeecae09b.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 24,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 1269,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/0d0a7e7d40a16ae6850d19f5e8704d8e.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/8b9328496990357033d4259fda250679.png",
      "retail_price": 899,
      "sell_volume": 205,
      "primary_product_id": 1029006,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "限时购",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 203,
      "is_hot": 0
    },
    {
      "id": 1030003,
      "category_id": 1008002,
      "goods_sn": "1030003",
      "name": "160*230羊毛手工几何地毯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "几何图案，打造立体的时尚感",
      "goods_desc": "<p><video id=\"tmpVedio0\" class=\"edui-upload-video video-js vjs-default-skin video-js\" controls=\"\" preload=\"auto\" width=\"100%\" height=\"\" data-setup=\"{}\"><source src=\"http://yanxuan.nosdn.127.net/e07746a58f5814648229ab750f7e59b0.mp4\" type=\"video/mp4\"/></video>‍</p><p><img src=\"http://yanxuan.nosdn.127.net/a03425edf97e1b0299d3095172991847.jpg\" _src=\"http://yanxuan.nosdn.127.net/a03425edf97e1b0299d3095172991847.jpg\" style=\"line-height: 1.42857;\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3fc35db4f3956b210032f0a876c2f2e.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3fc35db4f3956b210032f0a876c2f2e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf278ec3726e12e0a07ef4384f80d7c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf278ec3726e12e0a07ef4384f80d7c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/04cdc7e09537f67a140f5bd363751d23.jpg\" _src=\"http://yanxuan.nosdn.127.net/04cdc7e09537f67a140f5bd363751d23.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f4978e0569025d98c7a0cc685a3227d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/f4978e0569025d98c7a0cc685a3227d5.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/667999a8913e0dfc5118695f690f9ac4.jpg\" _src=\"http://yanxuan.nosdn.127.net/667999a8913e0dfc5118695f690f9ac4.jpg\" style=\"\"/></p><p><br/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0fe6f158bf93e05ae12fbc86ad7df61.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0fe6f158bf93e05ae12fbc86ad7df61.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39b84d98bfcbc4f0443ec04e39328d04.jpg\" _src=\"http://yanxuan.nosdn.127.net/39b84d98bfcbc4f0443ec04e39328d04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16218f2ea0f8f4ddfd1fcbeac17d3b54.jpg\" _src=\"http://yanxuan.nosdn.127.net/16218f2ea0f8f4ddfd1fcbeac17d3b54.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e512605b0a5ee1dea333c42f826050b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e512605b0a5ee1dea333c42f826050b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/001d8961d92c3ebcf860e1745d0c63b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/001d8961d92c3ebcf860e1745d0c63b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25dda9b93dd3dd9aa622779c27481ef4.jpg\" _src=\"http://yanxuan.nosdn.127.net/25dda9b93dd3dd9aa622779c27481ef4.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/037abff9d64cdc761092d47619df82d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/037abff9d64cdc761092d47619df82d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f755e4142e8baf68fab301b3e6438d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f755e4142e8baf68fab301b3e6438d5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa9ac1211dca7edc8fd93efd9cdd66e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa9ac1211dca7edc8fd93efd9cdd66e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ada62ef76b083d844d0762d2a6d33824.jpg\" _src=\"http://yanxuan.nosdn.127.net/ada62ef76b083d844d0762d2a6d33824.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 23,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/d74913e762fa11a4e27b0a20b8dad02d.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/1d1ab099dc0e254c15e57302e78e200b.png",
      "retail_price": 1469,
      "sell_volume": 464,
      "primary_product_id": 1029008,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1035006,
      "category_id": 1008002,
      "goods_sn": "1035006",
      "name": "全棉单面割绒浴室地垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "手工制作，纯棉材质，柔软舒适",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/39cba017dbf04371863ec3af894cb79c.jpg\" _src=\"http://yanxuan.nosdn.127.net/39cba017dbf04371863ec3af894cb79c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/727bdb71768265b3c283b2d71ad63d8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/727bdb71768265b3c283b2d71ad63d8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b7eb8df6b30b61ff8326a5882bbf411.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b7eb8df6b30b61ff8326a5882bbf411.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5143f756b613c2523954affbdf514a05.jpg\" _src=\"http://yanxuan.nosdn.127.net/5143f756b613c2523954affbdf514a05.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5a6879162b60e2442036c6c5d88275e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/5a6879162b60e2442036c6c5d88275e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d65d49dfd73f6b44d8e1b971df58ec1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/d65d49dfd73f6b44d8e1b971df58ec1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/630c9a177eb89c044d4c968745fce915.jpg\" _src=\"http://yanxuan.nosdn.127.net/630c9a177eb89c044d4c968745fce915.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1597a314b6ae69f361f4f1fbc2ed876c.jpg\" _src=\"http://yanxuan.nosdn.127.net/1597a314b6ae69f361f4f1fbc2ed876c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cfcfff37b305dcc44d9a907377761f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cfcfff37b305dcc44d9a907377761f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27dd23d01d9d110ebb11c92fa087e208.jpg\" _src=\"http://yanxuan.nosdn.127.net/27dd23d01d9d110ebb11c92fa087e208.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/366f5281836ad5b3a06afe4ace14d2bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/366f5281836ad5b3a06afe4ace14d2bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cdd2229692184db4793f68ca2d1c307.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cdd2229692184db4793f68ca2d1c307.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/999c7854dff1496c2702c510b8c6586d.jpg\" _src=\"http://yanxuan.nosdn.127.net/999c7854dff1496c2702c510b8c6586d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7097f2a9c69c4f337ab9ff961276cf0a.jpg\" _src=\"http://yanxuan.nosdn.127.net/7097f2a9c69c4f337ab9ff961276cf0a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d6ad8caac9c24f024b9525e492dde1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d6ad8caac9c24f024b9525e492dde1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1005834f8ac736dc7bc5c59cfab0ce01.jpg\" _src=\"http://yanxuan.nosdn.127.net/1005834f8ac736dc7bc5c59cfab0ce01.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/342365052bc031f64050c0d117786de1.jpg\" _src=\"http://yanxuan.nosdn.127.net/342365052bc031f64050c0d117786de1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bdb057b4b109ad39368d337b26fcef0.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bdb057b4b109ad39368d337b26fcef0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c764541e44c1bfe9308c4be9ba70eb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c764541e44c1bfe9308c4be9ba70eb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e4dafc25a731ccf56b1296e9889530d.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e4dafc25a731ccf56b1296e9889530d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0aae3c93d54fd9a25fc0d297e0cf856e.jpg\" _src=\"http://yanxuan.nosdn.127.net/0aae3c93d54fd9a25fc0d297e0cf856e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d3f4adea81508c83148517b12b3963f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d3f4adea81508c83148517b12b3963f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7f792a547c9f534fd4bd00c88fe734c.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7f792a547c9f534fd4bd00c88fe734c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41541dc15fbb715ed5311d4343516a6e.jpg\" _src=\"http://yanxuan.nosdn.127.net/41541dc15fbb715ed5311d4343516a6e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/267175ffcb24b51250f642b31cadd977.jpg\" _src=\"http://yanxuan.nosdn.127.net/267175ffcb24b51250f642b31cadd977.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 32,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 69,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/96b3f9af4a260902e7b8b3100af1da07.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ee92704f3b8323905b51fc647823e6e5.png",
      "retail_price": 56,
      "sell_volume": 14584,
      "primary_product_id": 1034011,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "限时购",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 203,
      "is_hot": 0
    },
    {
      "id": 1039051,
      "category_id": 1008002,
      "goods_sn": "1039051",
      "name": "多功能午睡枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "放松自在的午后时光",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/aba5fac220a511eb859ad4834fd7c0e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/aba5fac220a511eb859ad4834fd7c0e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37c7411fe03ac22b8b924190a5c6f483.jpg\" _src=\"http://yanxuan.nosdn.127.net/37c7411fe03ac22b8b924190a5c6f483.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88e313d81b848936d673edebc823f617.jpg\" _src=\"http://yanxuan.nosdn.127.net/88e313d81b848936d673edebc823f617.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/efddbb9e7105a72fb40f168813764297.jpg\" _src=\"http://yanxuan.nosdn.127.net/efddbb9e7105a72fb40f168813764297.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4830e1927e472f45940a92acf3e04331.jpg\" _src=\"http://yanxuan.nosdn.127.net/4830e1927e472f45940a92acf3e04331.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10b2f2989c7239bcea42be91d1826fc7.jpg\" _src=\"http://yanxuan.nosdn.127.net/10b2f2989c7239bcea42be91d1826fc7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3d19a5320eb179b3752458f15f1a068.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3d19a5320eb179b3752458f15f1a068.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97a9d81d01cbc6c8bf57e8b308de1537.jpg\" _src=\"http://yanxuan.nosdn.127.net/97a9d81d01cbc6c8bf57e8b308de1537.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/500497dcf877fbf29548ef7eae7766fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/500497dcf877fbf29548ef7eae7766fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92f6105f284bdd94aa4b6495a7d43994.jpg\" _src=\"http://yanxuan.nosdn.127.net/92f6105f284bdd94aa4b6495a7d43994.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60161ebc38b0b8c8ca9de8a0165843bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/60161ebc38b0b8c8ca9de8a0165843bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ce9817e2d4415c5789028c57c593450.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ce9817e2d4415c5789028c57c593450.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e3dc4f7c9dcd228a94cc4ffa6cea1be.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e3dc4f7c9dcd228a94cc4ffa6cea1be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89360198abf4bbb4c108bfe1068d83b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/89360198abf4bbb4c108bfe1068d83b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f40b5ba3618e61e80ad8f175b3da866.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f40b5ba3618e61e80ad8f175b3da866.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad590b8d9cb20c046d0d8e68ea3b0dc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad590b8d9cb20c046d0d8e68ea3b0dc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c606522a6032f1a2268a0ee0d8d01dff.jpg\" _src=\"http://yanxuan.nosdn.127.net/c606522a6032f1a2268a0ee0d8d01dff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f226b9e158f2cf451e925a606d1b5ecd.jpg\" _src=\"http://yanxuan.nosdn.127.net/f226b9e158f2cf451e925a606d1b5ecd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b169357e50d02d557c468588939c7f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b169357e50d02d557c468588939c7f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5e676b79ffc838a2c496134c8c3f55f.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5e676b79ffc838a2c496134c8c3f55f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e934b380901ffa4b035825b82246634e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e934b380901ffa4b035825b82246634e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8decfed210a7ada28bd71496a8ef51a.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8decfed210a7ada28bd71496a8ef51a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fcc94c2ee6ea13ef7cd7d21f1c63b79.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fcc94c2ee6ea13ef7cd7d21f1c63b79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8bae5453415f2fd519b5cf836e9baddc.jpg\" _src=\"http://yanxuan.nosdn.127.net/8bae5453415f2fd519b5cf836e9baddc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5833f7b80c040d8bdf23e514d430e045.jpg\" _src=\"http://yanxuan.nosdn.127.net/5833f7b80c040d8bdf23e514d430e045.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15df0095ff692e8d67185c93c44680c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/15df0095ff692e8d67185c93c44680c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32fdd19de26dee3281e76dc33059b1f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/32fdd19de26dee3281e76dc33059b1f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/290d679b2fe2154ef36b777525d988bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/290d679b2fe2154ef36b777525d988bc.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99233a211060d951818a729d43bb6533.jpg\" _src=\"http://yanxuan.nosdn.127.net/99233a211060d951818a729d43bb6533.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76fcb532c1aa2f631c0e439f5986654f.jpg\" _src=\"http://yanxuan.nosdn.127.net/76fcb532c1aa2f631c0e439f5986654f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2e90d2089e907d605e1eee0e6fcb1d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2e90d2089e907d605e1eee0e6fcb1d1.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 14,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/20e7e05935a347b36adac369efc490c3.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/c8ca0600fa7ba11ca8be6a3173dd38c9.png",
      "retail_price": 79,
      "sell_volume": 8202,
      "primary_product_id": 1038068,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1043005,
      "category_id": 1008002,
      "goods_sn": "1043005",
      "name": "日式记忆绵坐垫",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "活性炭记忆绵，缓解压力",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/7239e35762ea2937549f53f4482124fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/7239e35762ea2937549f53f4482124fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c23c022ad6737aa351140d7ce97a4a43.jpg\" _src=\"http://yanxuan.nosdn.127.net/c23c022ad6737aa351140d7ce97a4a43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b6fe3f499101077e6ee595a9145172c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b6fe3f499101077e6ee595a9145172c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fdc843045b99838abd8ce3fcbec2890.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fdc843045b99838abd8ce3fcbec2890.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14d3e1c384f5bc66e85b4dfff61f49ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/14d3e1c384f5bc66e85b4dfff61f49ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14eed3d4524fe441a54b604f37cfd299.jpg\" _src=\"http://yanxuan.nosdn.127.net/14eed3d4524fe441a54b604f37cfd299.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1b3a30c34e6fecf8105bf430e6d547f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1b3a30c34e6fecf8105bf430e6d547f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb5411b150ce5a69c0f88ef3af918061.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb5411b150ce5a69c0f88ef3af918061.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aebe8243acfa28a42d300d985c6e7036.jpg\" _src=\"http://yanxuan.nosdn.127.net/aebe8243acfa28a42d300d985c6e7036.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1371f124f86fc38c195f49e4bf26ddc5.jpg\" _src=\"http://yanxuan.nosdn.127.net/1371f124f86fc38c195f49e4bf26ddc5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd05471ebf5529464c85eace3e7c5c7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd05471ebf5529464c85eace3e7c5c7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c607e963758e4ad3f3bc749098fdcec.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c607e963758e4ad3f3bc749098fdcec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd472e779f1748937d269b87464722b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd472e779f1748937d269b87464722b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d19ec3e68922cdae4da8c0ab174bf5eb.jpg\" _src=\"http://yanxuan.nosdn.127.net/d19ec3e68922cdae4da8c0ab174bf5eb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44003fe38ab817003cb441ed5e518c41.jpg\" _src=\"http://yanxuan.nosdn.127.net/44003fe38ab817003cb441ed5e518c41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f3a7c45c70930950e60ddac979953d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f3a7c45c70930950e60ddac979953d5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77fc74a83c328dddf610a045277f094e.jpg\" _src=\"http://yanxuan.nosdn.127.net/77fc74a83c328dddf610a045277f094e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14056056c8e8cf3f77a479de696d18ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/14056056c8e8cf3f77a479de696d18ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ec2764b8b29c67af332cc1fde825b70.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ec2764b8b29c67af332cc1fde825b70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/494504fdb2d59d924de16cf79629dee9.jpg\" _src=\"http://yanxuan.nosdn.127.net/494504fdb2d59d924de16cf79629dee9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddf59afdada25b6b7aad72aaf8f0af20.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddf59afdada25b6b7aad72aaf8f0af20.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b8ad80c319aac920f3409bcd4376e17.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b8ad80c319aac920f3409bcd4376e17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8571525a4f280d09926a1b388d06fe8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/8571525a4f280d09926a1b388d06fe8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23c8bb2834f9ec05adb69e4df8354224.jpg\" _src=\"http://yanxuan.nosdn.127.net/23c8bb2834f9ec05adb69e4df8354224.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9c44aea67b0392547fdb3ba7f24c5fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9c44aea67b0392547fdb3ba7f24c5fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5045464902396b85ea12724ed962d7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5045464902396b85ea12724ed962d7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f484b21d07738839d1e199d8ba1031f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/f484b21d07738839d1e199d8ba1031f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21718c637256576c66876aa30653e29d.jpg\" _src=\"http://yanxuan.nosdn.127.net/21718c637256576c66876aa30653e29d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 11,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/aedfe3b7d76361d104a425ff551ade77.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/2a95b16f5b147cab4845641bee738a2e.png",
      "retail_price": 59,
      "sell_volume": 7482,
      "primary_product_id": 1041015,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1048005,
      "category_id": 1008002,
      "goods_sn": "1048005",
      "name": "日式色织水洗条纹抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "色织面料，水洗工艺，柔软亲肤",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/39afc6f165cf752e16c199b65ab61ee8.jpg\" _src=\"http://yanxuan.nosdn.127.net/39afc6f165cf752e16c199b65ab61ee8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2635f2eb08e98687a132a97642d87de.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2635f2eb08e98687a132a97642d87de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08b6bca750a85d833740e1f12e5a6216.jpg\" _src=\"http://yanxuan.nosdn.127.net/08b6bca750a85d833740e1f12e5a6216.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f61f9587dc8aec8330335da87dbb60ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/f61f9587dc8aec8330335da87dbb60ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f22282ebbbeb664ba706e4f088c9db2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/f22282ebbbeb664ba706e4f088c9db2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad7819c5597db9fce742cbc61aa53c72.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad7819c5597db9fce742cbc61aa53c72.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ee4a43824784e660f44e16274c4717ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/ee4a43824784e660f44e16274c4717ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f0eb752fd857fa1af74602afadabb0fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/f0eb752fd857fa1af74602afadabb0fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/46290c0b824babab46ce73feb23a554d.jpg\" _src=\"http://yanxuan.nosdn.127.net/46290c0b824babab46ce73feb23a554d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1c34134e19df505b4b1b2277880bba2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1c34134e19df505b4b1b2277880bba2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0bce553f09f5146ba9209264c46e38ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/0bce553f09f5146ba9209264c46e38ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/732ed69a0539f4d972213ed64e5bcff0.jpg\" _src=\"http://yanxuan.nosdn.127.net/732ed69a0539f4d972213ed64e5bcff0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/147fcd503618a36a76ed792c6a2254b1.jpg\" _src=\"http://yanxuan.nosdn.127.net/147fcd503618a36a76ed792c6a2254b1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f68cea7d1e7dd23349f7c36e366cb6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f68cea7d1e7dd23349f7c36e366cb6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/852711207b87360d29289be16a76e5ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/852711207b87360d29289be16a76e5ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f46c1d0edb91be4fa7c2747b423c494.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f46c1d0edb91be4fa7c2747b423c494.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f2bc29d55899694b917c9991d0b1333.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f2bc29d55899694b917c9991d0b1333.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63d4fa2caa8bbd1d7e205e90fe176633.jpg\" _src=\"http://yanxuan.nosdn.127.net/63d4fa2caa8bbd1d7e205e90fe176633.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f885db84f7911c3c4abc9695f55f19f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/f885db84f7911c3c4abc9695f55f19f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd0c5be6c986a60a577ab7fd4fa9796e.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd0c5be6c986a60a577ab7fd4fa9796e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb0f814679347c4876f2ca30acd57f88.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb0f814679347c4876f2ca30acd57f88.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/64b5936ea7e076885a7c1611d492aa57.jpg\" _src=\"http://yanxuan.nosdn.127.net/64b5936ea7e076885a7c1611d492aa57.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b503dd5b259a049dc3fffcabe6264c10.jpg\" _src=\"http://yanxuan.nosdn.127.net/b503dd5b259a049dc3fffcabe6264c10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3fb47a70640f6c252518a80a803bd362.jpg\" _src=\"http://yanxuan.nosdn.127.net/3fb47a70640f6c252518a80a803bd362.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1837c9a132b1ca0ed52f76f935563b7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1837c9a132b1ca0ed52f76f935563b7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09e9cc037e909c934aba0b87c48914ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/09e9cc037e909c934aba0b87c48914ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5c3a85ee4217386a8161016aa7727b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5c3a85ee4217386a8161016aa7727b9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e666622ecebc8fc733a49c5ad7d16c3e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e666622ecebc8fc733a49c5ad7d16c3e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48f87049ad7e2492ae75da78b97cd6fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/48f87049ad7e2492ae75da78b97cd6fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21cc4790d10496f2e73531c420fbb394.jpg\" _src=\"http://yanxuan.nosdn.127.net/21cc4790d10496f2e73531c420fbb394.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9510a74920b5589cba7af910774f8c0c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9510a74920b5589cba7af910774f8c0c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c69b713c98187890316668d10aa55c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c69b713c98187890316668d10aa55c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dcafde6d38fd075c4ba6d0cc1e816314.jpg\" _src=\"http://yanxuan.nosdn.127.net/dcafde6d38fd075c4ba6d0cc1e816314.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ccdf51824645c27ab06e78faa85db7d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ccdf51824645c27ab06e78faa85db7d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8096a502cac9f926d288cbbe8b8534fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/8096a502cac9f926d288cbbe8b8534fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b2b9a1f8a1422e3975cbee85685672c.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b2b9a1f8a1422e3975cbee85685672c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fd6779619cc7ed6f2a4057526f0c579d.jpg\" _src=\"http://yanxuan.nosdn.127.net/fd6779619cc7ed6f2a4057526f0c579d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdef4d1620407043511daf2e97746f07.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdef4d1620407043511daf2e97746f07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f30d798c772ea1599723c427c1d643b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f30d798c772ea1599723c427c1d643b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0cfc9aae9304010e24d92b29220dc0b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/0cfc9aae9304010e24d92b29220dc0b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e20e47f1eaf643bc569ccb148781529.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e20e47f1eaf643bc569ccb148781529.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9beb4226eb47be1c16e872dd9281634.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9beb4226eb47be1c16e872dd9281634.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70d2d737fbf7fc5980604ea294942b41.jpg\" _src=\"http://yanxuan.nosdn.127.net/70d2d737fbf7fc5980604ea294942b41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/496224b05a3054625b065de6aa769959.jpg\" _src=\"http://yanxuan.nosdn.127.net/496224b05a3054625b065de6aa769959.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0671941e0dfb696d5392f174a949a13.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0671941e0dfb696d5392f174a949a13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2df72e131e86e433d939776783a44db7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2df72e131e86e433d939776783a44db7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3bea99ca3040befe69d4811e0ef9b226.jpg\" _src=\"http://yanxuan.nosdn.127.net/3bea99ca3040befe69d4811e0ef9b226.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbc003f18889ab46a5a3a7e8698df351.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbc003f18889ab46a5a3a7e8698df351.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ee0df8d583844e734273d73eb582a4a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ee0df8d583844e734273d73eb582a4a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ea9467e6f4ef5c8f0812c1595704840.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ea9467e6f4ef5c8f0812c1595704840.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 5,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2167445c1b3df028d660bb992f321396.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ce980c16810a471dffff6aa8d7bac754.png",
      "retail_price": 59,
      "sell_volume": 5846,
      "primary_product_id": 1047014,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1055012,
      "category_id": 1008002,
      "goods_sn": "1055012",
      "name": "300根全棉羽丝绒抱枕芯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "仪征3D填充，充实的满足感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/07f2717762df73a6a697bb5399da6376.jpg\" _src=\"http://yanxuan.nosdn.127.net/07f2717762df73a6a697bb5399da6376.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e202bdb4be8f36bda118cf7265d00f65.jpg\" _src=\"http://yanxuan.nosdn.127.net/e202bdb4be8f36bda118cf7265d00f65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b5766cf268d327a3518ee5429c4c4e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b5766cf268d327a3518ee5429c4c4e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f4e4356d070dbca22cf19a60a2447ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f4e4356d070dbca22cf19a60a2447ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da3a3e22d355ccf82235603507f3a083.jpg\" _src=\"http://yanxuan.nosdn.127.net/da3a3e22d355ccf82235603507f3a083.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be789777e5e1381bb7b62d26fcfb619e.jpg\" _src=\"http://yanxuan.nosdn.127.net/be789777e5e1381bb7b62d26fcfb619e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c48e78aa87b8e81eab6a60de74d1c19c.jpg\" _src=\"http://yanxuan.nosdn.127.net/c48e78aa87b8e81eab6a60de74d1c19c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f772f4990d8ae0acac660acf25be2d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f772f4990d8ae0acac660acf25be2d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f1bd930fcb57e79a4ce2a1c4a0f2f4c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f1bd930fcb57e79a4ce2a1c4a0f2f4c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f481e1e9b8c4e728f4f7225af52a335e.jpg\" _src=\"http://yanxuan.nosdn.127.net/f481e1e9b8c4e728f4f7225af52a335e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4fca69439b053b510724cf6834856a2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/4fca69439b053b510724cf6834856a2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a285ec5ac9c84a6616feca7301f515c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a285ec5ac9c84a6616feca7301f515c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52435458ac1c48fb45f4a9888052b5b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/52435458ac1c48fb45f4a9888052b5b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/01301675d00e13d21588d0bbb72e1745.jpg\" _src=\"http://yanxuan.nosdn.127.net/01301675d00e13d21588d0bbb72e1745.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63627106753f764733cf47047e887d1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/63627106753f764733cf47047e887d1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15ecf40c8045513fe6a1303fe7d4383f.jpg\" _src=\"http://yanxuan.nosdn.127.net/15ecf40c8045513fe6a1303fe7d4383f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e8ef113464ff066662e639868e6eda28.jpg\" _src=\"http://yanxuan.nosdn.127.net/e8ef113464ff066662e639868e6eda28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0de1977400dfda99d0601e1c12fdbf1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/0de1977400dfda99d0601e1c12fdbf1e.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 10,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/06930cbd3bcd7c98d7740c18a7986137.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/3d437c8d68e2ec3f3dd61001bf98f16e.png",
      "retail_price": 39,
      "sell_volume": 6669,
      "primary_product_id": 1056022,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1055016,
      "category_id": 1008002,
      "goods_sn": "1055016",
      "name": "日式纯棉针织条纹抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "亲肤舒适，宛如妈妈的怀抱",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/4060bcde249c2501e5d95cfa0888a6c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/4060bcde249c2501e5d95cfa0888a6c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afebd965217cfdbc238de9252c7d6e37.jpg\" _src=\"http://yanxuan.nosdn.127.net/afebd965217cfdbc238de9252c7d6e37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b017649229c04dad59c312b3fe0cf7be.jpg\" _src=\"http://yanxuan.nosdn.127.net/b017649229c04dad59c312b3fe0cf7be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e02d923a92d5bef4b264381cffd5d813.jpg\" _src=\"http://yanxuan.nosdn.127.net/e02d923a92d5bef4b264381cffd5d813.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0447366651e06dde345c907e12315c73.jpg\" _src=\"http://yanxuan.nosdn.127.net/0447366651e06dde345c907e12315c73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5fdb8a54a2bc2285d1136bf9a2a674f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5fdb8a54a2bc2285d1136bf9a2a674f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1836dd3b75444a3ce42dc49fa5ee513.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1836dd3b75444a3ce42dc49fa5ee513.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f4740ae47c3ca8465e1ea6ec0a43563.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f4740ae47c3ca8465e1ea6ec0a43563.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f9f33a85933788209e6195468044387.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f9f33a85933788209e6195468044387.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b6ceab4330e0dd218db3c16582465be1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b6ceab4330e0dd218db3c16582465be1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dea7df197ba1e5ce5e9646aea43f798.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dea7df197ba1e5ce5e9646aea43f798.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/022e305413c9aa8e8db30a46a2a65286.jpg\" _src=\"http://yanxuan.nosdn.127.net/022e305413c9aa8e8db30a46a2a65286.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cce2571a59a0bc39784d61c4134f9458.jpg\" _src=\"http://yanxuan.nosdn.127.net/cce2571a59a0bc39784d61c4134f9458.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1f287dab80d1b11450051de6c119611.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1f287dab80d1b11450051de6c119611.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7b6318cb7623349542ba971cf1887da.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7b6318cb7623349542ba971cf1887da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf56a8ae91e07c91d70cf7b88cb59676.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf56a8ae91e07c91d70cf7b88cb59676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76aebdbc4a150837b2dcaa2293c85cc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/76aebdbc4a150837b2dcaa2293c85cc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/902fb302066a65488ed1f6da3a16ed66.jpg\" _src=\"http://yanxuan.nosdn.127.net/902fb302066a65488ed1f6da3a16ed66.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd9df2852e760940b0ab9e599320ed35.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd9df2852e760940b0ab9e599320ed35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ad1c6c9e619df09685cf9596339d714.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ad1c6c9e619df09685cf9596339d714.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83e54a3b9d13dc3c67e880c02e63167c.jpg\" _src=\"http://yanxuan.nosdn.127.net/83e54a3b9d13dc3c67e880c02e63167c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f6b75fe4ff9ae0b976c8c85bbf0a719.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f6b75fe4ff9ae0b976c8c85bbf0a719.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82f850ea52ca3e7048283b3f8a65c616.jpg\" _src=\"http://yanxuan.nosdn.127.net/82f850ea52ca3e7048283b3f8a65c616.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5bd4faa4898d9ea3c56fba9c5749cc62.jpg\" _src=\"http://yanxuan.nosdn.127.net/5bd4faa4898d9ea3c56fba9c5749cc62.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6488dedf51c6e5a90fc5f156a4e8416b.jpg\" _src=\"http://yanxuan.nosdn.127.net/6488dedf51c6e5a90fc5f156a4e8416b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bc667ddb5116ceaf329f55982da36bb1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bc667ddb5116ceaf329f55982da36bb1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfbfde943773a0258fa81b84d710d36e.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfbfde943773a0258fa81b84d710d36e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60d64bb0ac51346dc39d266beacdb846.jpg\" _src=\"http://yanxuan.nosdn.127.net/60d64bb0ac51346dc39d266beacdb846.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c50c0fd364d6b9a8646d0da75ce48f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c50c0fd364d6b9a8646d0da75ce48f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b24da9df819efdf9e110bb2228eadf0d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b24da9df819efdf9e110bb2228eadf0d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3cbbd9ec8dd41be2b35bf49842b67d86.jpg\" _src=\"http://yanxuan.nosdn.127.net/3cbbd9ec8dd41be2b35bf49842b67d86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d5bb53b92ed48f3f81980e41b51c0fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d5bb53b92ed48f3f81980e41b51c0fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d75a8fd77357f9a74a36fd7bfa7cebed.jpg\" _src=\"http://yanxuan.nosdn.127.net/d75a8fd77357f9a74a36fd7bfa7cebed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2dd8069e6739d732a53c25c74c0b2a89.jpg\" _src=\"http://yanxuan.nosdn.127.net/2dd8069e6739d732a53c25c74c0b2a89.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d7b4e172f8fd168e28854c3d8d04c56f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d7b4e172f8fd168e28854c3d8d04c56f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8b981b58ffb3e0a75916def11e45493.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8b981b58ffb3e0a75916def11e45493.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fb12dd3d12c8828a5cf2e16f17a8f27.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fb12dd3d12c8828a5cf2e16f17a8f27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8df57201eb9f5e7b576a6ccc31286e8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8df57201eb9f5e7b576a6ccc31286e8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f86f20ab83206abfdd682418e3cd3ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f86f20ab83206abfdd682418e3cd3ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c64ea783c9bd6dd2cb51b9978769edb.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c64ea783c9bd6dd2cb51b9978769edb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/104dca8bdfb6413fed5379a5b04eec10.jpg\" _src=\"http://yanxuan.nosdn.127.net/104dca8bdfb6413fed5379a5b04eec10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2cfb7760b81f0a82bdbae5079bfcd5ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/2cfb7760b81f0a82bdbae5079bfcd5ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1c6e09984c0599b5205f4d099cd5cfcb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1c6e09984c0599b5205f4d099cd5cfcb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e32f3a0bbc7ba3ec49b69fa89ba7da39.jpg\" _src=\"http://yanxuan.nosdn.127.net/e32f3a0bbc7ba3ec49b69fa89ba7da39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/408bf6b2815efea1020278ff57204667.jpg\" _src=\"http://yanxuan.nosdn.127.net/408bf6b2815efea1020278ff57204667.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6707b10b7a14f7d2e7487f30a687cfb2.jpg\" _src=\"http://yanxuan.nosdn.127.net/6707b10b7a14f7d2e7487f30a687cfb2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c4977d2ce8691f85575698990c13c3a.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c4977d2ce8691f85575698990c13c3a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22213164e3ce12c23260519cc5f2dd7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/22213164e3ce12c23260519cc5f2dd7f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9c8f7fda81f79cec8e75404386677c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9c8f7fda81f79cec8e75404386677c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1e5093b54f817ed1906fc58e7494790.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1e5093b54f817ed1906fc58e7494790.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/162452d2cb5ad3348862d5b1da7348c5.jpg\" _src=\"http://yanxuan.nosdn.127.net/162452d2cb5ad3348862d5b1da7348c5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8f6de9bc947bed7d5cebfe1f49a786d.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8f6de9bc947bed7d5cebfe1f49a786d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 8,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/8132003a8940c7056960c3c5fce59903.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/23e0203f1512f33e605f61c28fa03d2d.png",
      "retail_price": 59,
      "sell_volume": 948,
      "primary_product_id": 1056032,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1057036,
      "category_id": 1008002,
      "goods_sn": "1057036",
      "name": "日式纯色水洗亚麻抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "水洗亚麻，透气亲肤",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/6b69f7597ccffd27d77467d9d04eb294.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b69f7597ccffd27d77467d9d04eb294.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a89ca371ef07355c1feb293db961bd30.jpg\" _src=\"http://yanxuan.nosdn.127.net/a89ca371ef07355c1feb293db961bd30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2076e89c5f8fde4f44f918bd02d18eb7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2076e89c5f8fde4f44f918bd02d18eb7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5c9111e4dcc13cb41db98f68086cc620.jpg\" _src=\"http://yanxuan.nosdn.127.net/5c9111e4dcc13cb41db98f68086cc620.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f0645abcf883e7a863f32ce95f3c26b.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f0645abcf883e7a863f32ce95f3c26b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76a2b12f2d0f48f268d18b0ca0d1d6bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/76a2b12f2d0f48f268d18b0ca0d1d6bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a91f75159867f33a91f4e9992e00afa1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a91f75159867f33a91f4e9992e00afa1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93de61256a8ff3a8aa4bb90847ff454e.jpg\" _src=\"http://yanxuan.nosdn.127.net/93de61256a8ff3a8aa4bb90847ff454e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f611f99bea2920881e1421c110970234.jpg\" _src=\"http://yanxuan.nosdn.127.net/f611f99bea2920881e1421c110970234.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a292339423f141ad5d7a4011ea316956.jpg\" _src=\"http://yanxuan.nosdn.127.net/a292339423f141ad5d7a4011ea316956.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2045ae4f861d9eae6af351b9d82c9239.jpg\" _src=\"http://yanxuan.nosdn.127.net/2045ae4f861d9eae6af351b9d82c9239.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/398718a6d579c4af5f255909283e44a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/398718a6d579c4af5f255909283e44a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5be95e2db627908d23605fe042af2937.jpg\" _src=\"http://yanxuan.nosdn.127.net/5be95e2db627908d23605fe042af2937.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50a4fa0f67aa85dfaad36695225fe2f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/50a4fa0f67aa85dfaad36695225fe2f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c825e297cfbaaae632146a55c61dc3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c825e297cfbaaae632146a55c61dc3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/261c7819e7e9ac165e64cae88a59f70c.jpg\" _src=\"http://yanxuan.nosdn.127.net/261c7819e7e9ac165e64cae88a59f70c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec83f40d91fcc79f59a2479dffeb4565.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec83f40d91fcc79f59a2479dffeb4565.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/26f3e85402086b7d261a650e244dc676.jpg\" _src=\"http://yanxuan.nosdn.127.net/26f3e85402086b7d261a650e244dc676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dccb68f0d97112d245ab1924744b94b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/dccb68f0d97112d245ab1924744b94b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaba69949efd7ed85e72071f4ade4945.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaba69949efd7ed85e72071f4ade4945.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f23300061e5cf871e86a51f0012e885.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f23300061e5cf871e86a51f0012e885.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a55eedca057e0c973549ac8f13b47800.jpg\" _src=\"http://yanxuan.nosdn.127.net/a55eedca057e0c973549ac8f13b47800.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abf16e831285e3d97dbb60a3162e7968.jpg\" _src=\"http://yanxuan.nosdn.127.net/abf16e831285e3d97dbb60a3162e7968.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9390c8dab9fc7d8c27ac9410eb0340c.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9390c8dab9fc7d8c27ac9410eb0340c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8feb2be5afec5abe439cf1b42683373f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8feb2be5afec5abe439cf1b42683373f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/beb7620d0f685ab9c3af7ed18284b29e.jpg\" _src=\"http://yanxuan.nosdn.127.net/beb7620d0f685ab9c3af7ed18284b29e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f70ceed2078d44d747a9ce369feee9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f70ceed2078d44d747a9ce369feee9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5469e219bd5347568337746b257f094e.jpg\" _src=\"http://yanxuan.nosdn.127.net/5469e219bd5347568337746b257f094e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a177a6b6e58580809330895ebdbaff6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/a177a6b6e58580809330895ebdbaff6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9db0090d56ab757babb2ba661726cbe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/9db0090d56ab757babb2ba661726cbe3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6363637e0dd2fc670745c217b2a5cbfc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6363637e0dd2fc670745c217b2a5cbfc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1af1bde98f1497f591f62bff99ccca54.jpg\" _src=\"http://yanxuan.nosdn.127.net/1af1bde98f1497f591f62bff99ccca54.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69d034b353ae2e6e30afb6c21483690f.jpg\" _src=\"http://yanxuan.nosdn.127.net/69d034b353ae2e6e30afb6c21483690f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e29d6ac5ed040d63847ca456a179d43.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e29d6ac5ed040d63847ca456a179d43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29e460fba57f67cd83121f6cb917cfbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/29e460fba57f67cd83121f6cb917cfbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16090c02f4d4b76c6be82d98e489586e.jpg\" _src=\"http://yanxuan.nosdn.127.net/16090c02f4d4b76c6be82d98e489586e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c840eb66cf002227c52a13fbe55f657b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c840eb66cf002227c52a13fbe55f657b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16f65265b0942a60f3241704dc29be13.jpg\" _src=\"http://yanxuan.nosdn.127.net/16f65265b0942a60f3241704dc29be13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54a63da54b4e80867d8cd92d1ea9576e.jpg\" _src=\"http://yanxuan.nosdn.127.net/54a63da54b4e80867d8cd92d1ea9576e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebd0b906076850983e5a2aae9f667ce7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebd0b906076850983e5a2aae9f667ce7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bbf32cdc82643a85c12ff05ea88088ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/bbf32cdc82643a85c12ff05ea88088ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca6e3ccc3725c3f58338b62a5a0655d3.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca6e3ccc3725c3f58338b62a5a0655d3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ef02962e6155f811566aad168dabbec.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ef02962e6155f811566aad168dabbec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/832735166071f05288ffd347dff58ee6.jpg\" _src=\"http://yanxuan.nosdn.127.net/832735166071f05288ffd347dff58ee6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4fc490c4e9a0a0fa0affd317b8526f4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4fc490c4e9a0a0fa0affd317b8526f4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b05f975f16c09f106c81533c1a249b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b05f975f16c09f106c81533c1a249b0.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 6,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/f40fffd36cc85d5e0cf69417f4192ac1.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/8a9ee5ba08929cc9e40b973607d2f633.png",
      "retail_price": 79,
      "sell_volume": 1727,
      "primary_product_id": 1058097,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1072000,
      "category_id": 1008002,
      "goods_sn": "1072000",
      "name": "手工针织绞花抱枕套",
      "brand_id": 1001020,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "纯手工针织，带给你复古的暖",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/74ead5d764e22f8d50dc44a7a61da41a.jpg\" _src=\"http://yanxuan.nosdn.127.net/74ead5d764e22f8d50dc44a7a61da41a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be7f775d658e40e6ca76e657006053a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/be7f775d658e40e6ca76e657006053a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7fe9345385034a4d25580072444b349b.jpg\" _src=\"http://yanxuan.nosdn.127.net/7fe9345385034a4d25580072444b349b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bffafbafcf3010c3e5ab454af09cde4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/bffafbafcf3010c3e5ab454af09cde4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/123a0dcb707c2a178e5f9da395b5b24e.jpg\" _src=\"http://yanxuan.nosdn.127.net/123a0dcb707c2a178e5f9da395b5b24e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfeba71e7e71a63dee06b079b4c4c4f0.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfeba71e7e71a63dee06b079b4c4c4f0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cdc034602358c7752073a9b4bd6b499f.jpg\" _src=\"http://yanxuan.nosdn.127.net/cdc034602358c7752073a9b4bd6b499f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3050a816fd41ec2b8880d11aafc26177.jpg\" _src=\"http://yanxuan.nosdn.127.net/3050a816fd41ec2b8880d11aafc26177.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/027e8c218edbbf1779cf4b380b2133c2.jpg\" _src=\"http://yanxuan.nosdn.127.net/027e8c218edbbf1779cf4b380b2133c2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbd1f6dd39bd517c99c7ae07d9b32b0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbd1f6dd39bd517c99c7ae07d9b32b0e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db5baa7586787b7e0f27a5b7a09946a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/db5baa7586787b7e0f27a5b7a09946a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/66a0ff102559b2d840240d6fa8c37001.jpg\" _src=\"http://yanxuan.nosdn.127.net/66a0ff102559b2d840240d6fa8c37001.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b17b0772d947612819e4489d9e5a865.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b17b0772d947612819e4489d9e5a865.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53cc65ea58a7757fca2585b25056cf21.jpg\" _src=\"http://yanxuan.nosdn.127.net/53cc65ea58a7757fca2585b25056cf21.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/86506725ae85f9864c8b70b64b2e37d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/86506725ae85f9864c8b70b64b2e37d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/671d390a50d363d6ae6ab0c52f06a284.jpg\" _src=\"http://yanxuan.nosdn.127.net/671d390a50d363d6ae6ab0c52f06a284.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14e864b84a51faebab51912bbfea7b75.jpg\" _src=\"http://yanxuan.nosdn.127.net/14e864b84a51faebab51912bbfea7b75.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e31d1086f08b77298977c2b459be4833.jpg\" _src=\"http://yanxuan.nosdn.127.net/e31d1086f08b77298977c2b459be4833.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02338b650755a458ca8561f484e618d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/02338b650755a458ca8561f484e618d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ffbeafbda15fcfcf98c3b7a62c77e05.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ffbeafbda15fcfcf98c3b7a62c77e05.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f61f5e704ccf72bfb570842a366f104.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f61f5e704ccf72bfb570842a366f104.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e119daabcfd640441083e17445834954.jpg\" _src=\"http://yanxuan.nosdn.127.net/e119daabcfd640441083e17445834954.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/010ba3b486af23613c04046c5829a7c2.jpg\" _src=\"http://yanxuan.nosdn.127.net/010ba3b486af23613c04046c5829a7c2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25f470d4479fbb74f9b6e105f8dedfbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/25f470d4479fbb74f9b6e105f8dedfbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e7c300089dba380e9f48d49ec964ff9.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e7c300089dba380e9f48d49ec964ff9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a7ab3c980cf291404489bd137efde6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a7ab3c980cf291404489bd137efde6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2fb08e93fa462fca26680a56737b9f91.jpg\" _src=\"http://yanxuan.nosdn.127.net/2fb08e93fa462fca26680a56737b9f91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0ad6f5f75871fa02408723457a8a8ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0ad6f5f75871fa02408723457a8a8ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3cecb48c44520393993ce5bc85da7ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3cecb48c44520393993ce5bc85da7ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cd68c353ca83624fa367f90592649b36.jpg\" _src=\"http://yanxuan.nosdn.127.net/cd68c353ca83624fa367f90592649b36.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9327cc921602b9d5b05147e4266910cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/9327cc921602b9d5b05147e4266910cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37cf3aa662187aa1126a5c41cb41d796.jpg\" _src=\"http://yanxuan.nosdn.127.net/37cf3aa662187aa1126a5c41cb41d796.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bef5ea165cda6dbbb109ea895b3f2fc5.jpg\" _src=\"http://yanxuan.nosdn.127.net/bef5ea165cda6dbbb109ea895b3f2fc5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/78c0d06130500a1247cb2a602264c61c.jpg\" _src=\"http://yanxuan.nosdn.127.net/78c0d06130500a1247cb2a602264c61c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79fd1cbd0c0d02ac58c2f449dcb6c97f.jpg\" _src=\"http://yanxuan.nosdn.127.net/79fd1cbd0c0d02ac58c2f449dcb6c97f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61acb2d95e1833aad988c183c94eebe2.jpg\" _src=\"http://yanxuan.nosdn.127.net/61acb2d95e1833aad988c183c94eebe2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7828935cd158c7bb6643186eb25be8bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/7828935cd158c7bb6643186eb25be8bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0409cef7649088f345fc64a348b49468.jpg\" _src=\"http://yanxuan.nosdn.127.net/0409cef7649088f345fc64a348b49468.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54e1beab4c0616b3147270201f978f2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/54e1beab4c0616b3147270201f978f2d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a75d34f45de74f2476f34ce329d57ff6.jpg\" _src=\"http://yanxuan.nosdn.127.net/a75d34f45de74f2476f34ce329d57ff6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/81607103dfd183acf7a364dd58e3cf93.jpg\" _src=\"http://yanxuan.nosdn.127.net/81607103dfd183acf7a364dd58e3cf93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/03cf20624d36fc793143ba7ba8b5c17f.jpg\" _src=\"http://yanxuan.nosdn.127.net/03cf20624d36fc793143ba7ba8b5c17f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da92a3b8729effd6f79e9c86b522f6ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/da92a3b8729effd6f79e9c86b522f6ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71aa5c2a762f4bced311f40323980552.jpg\" _src=\"http://yanxuan.nosdn.127.net/71aa5c2a762f4bced311f40323980552.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b81f52020b75b35b2254d327625713d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/b81f52020b75b35b2254d327625713d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f4d245eea01d80ce6769f308ccd7152.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f4d245eea01d80ce6769f308ccd7152.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c74f125472bf12a5b0ece0aaf15ef85.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c74f125472bf12a5b0ece0aaf15ef85.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6139fdd3fb21d66c527520a747a17fe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/6139fdd3fb21d66c527520a747a17fe3.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 9,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/09883bdbd9eec88ed615b99a275c0d54.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/87cf3a17ad40bfdcdc3314ea4591a5e8.png",
      "retail_price": 89,
      "sell_volume": 305,
      "primary_product_id": 1076004,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1072001,
      "category_id": 1008002,
      "goods_sn": "1072001",
      "name": "色织水洗棉绣花抱枕套",
      "brand_id": 1001020,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "清素色织，搭配水洗棉旧色的温柔",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/f8a74bd8e87987849bf2505c08ac69e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8a74bd8e87987849bf2505c08ac69e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be7ae107fc4b5085241507ed711254f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/be7ae107fc4b5085241507ed711254f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/143c402e82c2d99c3bc7cc51d064a62b.jpg\" _src=\"http://yanxuan.nosdn.127.net/143c402e82c2d99c3bc7cc51d064a62b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52f5b211f5da083da2bc9b5237c40b3b.jpg\" _src=\"http://yanxuan.nosdn.127.net/52f5b211f5da083da2bc9b5237c40b3b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5af00c6f7dc0d798dffe2cdc2da0f870.jpg\" _src=\"http://yanxuan.nosdn.127.net/5af00c6f7dc0d798dffe2cdc2da0f870.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/750bbc1c2207159b58a6de350060f5c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/750bbc1c2207159b58a6de350060f5c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d55dd54de50ff03b199261f3e021f388.jpg\" _src=\"http://yanxuan.nosdn.127.net/d55dd54de50ff03b199261f3e021f388.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b659703ddf8e35bb89ee5ff36e84b4f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/b659703ddf8e35bb89ee5ff36e84b4f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/573f30d45c3eea65f29a6497ac2b9a98.jpg\" _src=\"http://yanxuan.nosdn.127.net/573f30d45c3eea65f29a6497ac2b9a98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7d58eb147f2d8bedfc88ba08b544d7c.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7d58eb147f2d8bedfc88ba08b544d7c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec89200168dd4a703f7b89ec2be0b8a4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec89200168dd4a703f7b89ec2be0b8a4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d123c7d7b79ef8cd2703976e8bf1dbc.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d123c7d7b79ef8cd2703976e8bf1dbc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2797ba305c10b0e5fd6eafb384101402.jpg\" _src=\"http://yanxuan.nosdn.127.net/2797ba305c10b0e5fd6eafb384101402.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abcfbdafabe855e77598860b426fa5e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/abcfbdafabe855e77598860b426fa5e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d6ff672dae187d85d199ee1b1b62f9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d6ff672dae187d85d199ee1b1b62f9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e4424539e51dca9d000c6b67bea1f8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e4424539e51dca9d000c6b67bea1f8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/942da4a7c05d2a25be7a26decc40f53a.jpg\" _src=\"http://yanxuan.nosdn.127.net/942da4a7c05d2a25be7a26decc40f53a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c872c106b7da7d7b1167a9554c92aa1.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c872c106b7da7d7b1167a9554c92aa1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82607c78aedacd534a2e0f1b38e2e3e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/82607c78aedacd534a2e0f1b38e2e3e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/07e4e5ac1501706c8666eff4a703b5fb.jpg\" _src=\"http://yanxuan.nosdn.127.net/07e4e5ac1501706c8666eff4a703b5fb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a56805f63dfe98583e6b58eaa9dd595a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a56805f63dfe98583e6b58eaa9dd595a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ecdd28de374db2de0c0c2f0f50d0cd26.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecdd28de374db2de0c0c2f0f50d0cd26.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69fcb2566dea15f16a182b7e4e05893f.jpg\" _src=\"http://yanxuan.nosdn.127.net/69fcb2566dea15f16a182b7e4e05893f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bc3c5b3a6a14c8307e57842bf737601b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bc3c5b3a6a14c8307e57842bf737601b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d9c980cc924790bd7983bd80b0221a.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d9c980cc924790bd7983bd80b0221a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/787bdee826a5112c3e2bd4b9c15717e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/787bdee826a5112c3e2bd4b9c15717e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44dc985f99b3a95f255624a4d97857ca.jpg\" _src=\"http://yanxuan.nosdn.127.net/44dc985f99b3a95f255624a4d97857ca.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf117d9aef1ef7ab10d2ef040d9444c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf117d9aef1ef7ab10d2ef040d9444c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/07044f1a6c11d8d15e410a01482fb39a.jpg\" _src=\"http://yanxuan.nosdn.127.net/07044f1a6c11d8d15e410a01482fb39a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ca8ea48405cb43c901181a684c623dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ca8ea48405cb43c901181a684c623dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b4111628661d4216c8d0fc057e6d81e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b4111628661d4216c8d0fc057e6d81e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4adb10168dbfcee6f49460b2478de249.jpg\" _src=\"http://yanxuan.nosdn.127.net/4adb10168dbfcee6f49460b2478de249.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e798dd4abe3a833a4d0066453955ec1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/e798dd4abe3a833a4d0066453955ec1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/528abeae19cf1b5af2f49be4e142a2da.jpg\" _src=\"http://yanxuan.nosdn.127.net/528abeae19cf1b5af2f49be4e142a2da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2d3d5ae118bcacdfda08eb182a03c15a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2d3d5ae118bcacdfda08eb182a03c15a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3323a393743f839e12586418a0711123.jpg\" _src=\"http://yanxuan.nosdn.127.net/3323a393743f839e12586418a0711123.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ac29c5a1569d9fb37420f2eae835b91.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ac29c5a1569d9fb37420f2eae835b91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89ef4f7ec1c86f13d328c23c0429892a.jpg\" _src=\"http://yanxuan.nosdn.127.net/89ef4f7ec1c86f13d328c23c0429892a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b005b97dbffa333e49ff484abbcff04.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b005b97dbffa333e49ff484abbcff04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afa56b9370cdc27f27f8f951108cea4c.jpg\" _src=\"http://yanxuan.nosdn.127.net/afa56b9370cdc27f27f8f951108cea4c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5daae71eb699e7417e695472e1142678.jpg\" _src=\"http://yanxuan.nosdn.127.net/5daae71eb699e7417e695472e1142678.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3dbb71ba9fff82849a959deb8f5b7946.jpg\" _src=\"http://yanxuan.nosdn.127.net/3dbb71ba9fff82849a959deb8f5b7946.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e024ba974bad906db9e2a28d42293a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e024ba974bad906db9e2a28d42293a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/87e2d46daab9e1dd3e112c15692c66ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/87e2d46daab9e1dd3e112c15692c66ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/342bc9bb1cbf81d1bc7b33f77fa915ff.jpg\" _src=\"http://yanxuan.nosdn.127.net/342bc9bb1cbf81d1bc7b33f77fa915ff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f54d685cb3c111beff7ef58bb16252d6.jpg\" _src=\"http://yanxuan.nosdn.127.net/f54d685cb3c111beff7ef58bb16252d6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7c4c896daa0ac2ff5f89d5b738fc007.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7c4c896daa0ac2ff5f89d5b738fc007.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/839da4fb5874271d54f94c60ad4d7387.jpg\" _src=\"http://yanxuan.nosdn.127.net/839da4fb5874271d54f94c60ad4d7387.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7147d5acd91c330479762e51cf4257f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/7147d5acd91c330479762e51cf4257f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a9ca13fd9189e60df2f4a21783a3795.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a9ca13fd9189e60df2f4a21783a3795.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09fa8e6e95cc716138549e6b244a7924.jpg\" _src=\"http://yanxuan.nosdn.127.net/09fa8e6e95cc716138549e6b244a7924.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/772e18352ad2c156ee190f068726cd8c.jpg\" _src=\"http://yanxuan.nosdn.127.net/772e18352ad2c156ee190f068726cd8c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92c0a1e57d429d19fb7f4e678fa7fae1.jpg\" _src=\"http://yanxuan.nosdn.127.net/92c0a1e57d429d19fb7f4e678fa7fae1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88ddae38e8b363acdf79bfbe0547cc50.jpg\" _src=\"http://yanxuan.nosdn.127.net/88ddae38e8b363acdf79bfbe0547cc50.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c4c683112a57543d4e028754be53e0d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c4c683112a57543d4e028754be53e0d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f476dbaf8a8cae1e8a311edb77d4ea78.jpg\" _src=\"http://yanxuan.nosdn.127.net/f476dbaf8a8cae1e8a311edb77d4ea78.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7493e6d2980dc116654bdb3b24c1a3d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7493e6d2980dc116654bdb3b24c1a3d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/57e84b0e4b979782b0c3a4bce908d797.jpg\" _src=\"http://yanxuan.nosdn.127.net/57e84b0e4b979782b0c3a4bce908d797.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8eb47f38c324fd320c74bf0aa3ebdf1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8eb47f38c324fd320c74bf0aa3ebdf1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/622949bf7e667ea54eaf0861ac31c842.jpg\" _src=\"http://yanxuan.nosdn.127.net/622949bf7e667ea54eaf0861ac31c842.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 7,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a45cf27cc07e678cfe21257cb764711a.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/0e9d5954d7dc2477d9c46b730e05ab42.png",
      "retail_price": 49,
      "sell_volume": 121,
      "primary_product_id": 1076007,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1081000,
      "category_id": 1008002,
      "goods_sn": "1081000",
      "name": "北欧风珊瑚绒多功能暖手枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "手枕坐垫两用",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/19ce01a5361a70388e7d40e94ccd3495.jpg\" _src=\"http://yanxuan.nosdn.127.net/19ce01a5361a70388e7d40e94ccd3495.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a037a815a9c11449de1c5c94d6a6d987.jpg\" _src=\"http://yanxuan.nosdn.127.net/a037a815a9c11449de1c5c94d6a6d987.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7ccc425d60247f8468ede401cb74683.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7ccc425d60247f8468ede401cb74683.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/039951ed06296e8065f7b219a4a111de.jpg\" _src=\"http://yanxuan.nosdn.127.net/039951ed06296e8065f7b219a4a111de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37576f4179798648632a694da355996f.jpg\" _src=\"http://yanxuan.nosdn.127.net/37576f4179798648632a694da355996f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d45db0fcfff3fb9ced3f6bc5e5d6a23.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d45db0fcfff3fb9ced3f6bc5e5d6a23.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e46450a60e9bc60bca3f483ad14337b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/e46450a60e9bc60bca3f483ad14337b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/071c557f2845aa18a7f4d80f556b1178.jpg\" _src=\"http://yanxuan.nosdn.127.net/071c557f2845aa18a7f4d80f556b1178.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5935e928d9b1b6781db188cf41f93424.jpg\" _src=\"http://yanxuan.nosdn.127.net/5935e928d9b1b6781db188cf41f93424.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83f8bac183a90e5d8f32c698813ef046.jpg\" _src=\"http://yanxuan.nosdn.127.net/83f8bac183a90e5d8f32c698813ef046.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7ae7816d84e084b9df010ae92f7c0bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7ae7816d84e084b9df010ae92f7c0bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c89f0917bceb94f0e300df77d08c75e.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c89f0917bceb94f0e300df77d08c75e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62c52e788f028eab5b4927671f4aa109.jpg\" _src=\"http://yanxuan.nosdn.127.net/62c52e788f028eab5b4927671f4aa109.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93b9efc4c1b39c065c0dde2974a9dc52.jpg\" _src=\"http://yanxuan.nosdn.127.net/93b9efc4c1b39c065c0dde2974a9dc52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40da45628d48712880dc64843aba8e6a.jpg\" _src=\"http://yanxuan.nosdn.127.net/40da45628d48712880dc64843aba8e6a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec12badecafb5dd8f67b52efa6cf4b15.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec12badecafb5dd8f67b52efa6cf4b15.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bde2888497b52e724ca72d42a86578d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bde2888497b52e724ca72d42a86578d1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f1b163294dff20ac85a5f6dc8016500.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f1b163294dff20ac85a5f6dc8016500.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f970069e7d381421dec8c407fcd2a7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f970069e7d381421dec8c407fcd2a7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b852d0821395488c729a4d09941b2ea7.jpg\" _src=\"http://yanxuan.nosdn.127.net/b852d0821395488c729a4d09941b2ea7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/660168255d39ded4c1d2038cff5d253f.jpg\" _src=\"http://yanxuan.nosdn.127.net/660168255d39ded4c1d2038cff5d253f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7fe09efd35ef54dfa0a92c8059971995.jpg\" _src=\"http://yanxuan.nosdn.127.net/7fe09efd35ef54dfa0a92c8059971995.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f13328e747638a9681502f97d0fc032a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f13328e747638a9681502f97d0fc032a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/05c538811b7d8d37b15e9b168b45ed19.jpg\" _src=\"http://yanxuan.nosdn.127.net/05c538811b7d8d37b15e9b168b45ed19.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e597815f2bbf76f2c078326d3cd255e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/e597815f2bbf76f2c078326d3cd255e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/73d7bd31e90a2bdc79263dde20e2496c.jpg\" _src=\"http://yanxuan.nosdn.127.net/73d7bd31e90a2bdc79263dde20e2496c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e10091f21b56c616ac4ab51decab76a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e10091f21b56c616ac4ab51decab76a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5023b92342a2f936996c2eaf2e79f1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5023b92342a2f936996c2eaf2e79f1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a090e4b9269a901e660cc35a1c38975a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a090e4b9269a901e660cc35a1c38975a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85c707ebaae017ab65bf5e2266ec7c6d.jpg\" _src=\"http://yanxuan.nosdn.127.net/85c707ebaae017ab65bf5e2266ec7c6d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/30a57bf64ad98af99955d90e45ae9f3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/30a57bf64ad98af99955d90e45ae9f3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ec59f055c27c776ee5ec635e1e64b79.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ec59f055c27c776ee5ec635e1e64b79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f39b93929486b2ba679ed22fac5021b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/f39b93929486b2ba679ed22fac5021b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ea9e76b9b0988c823796752cd3bc4e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ea9e76b9b0988c823796752cd3bc4e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b952cc40eab4b590943ad91fb35c4ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b952cc40eab4b590943ad91fb35c4ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f5e5f1d2adbb2aaaf10e1e38913206b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f5e5f1d2adbb2aaaf10e1e38913206b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50c14625bb7a2d0331fee4181ae22455.jpg\" _src=\"http://yanxuan.nosdn.127.net/50c14625bb7a2d0331fee4181ae22455.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7af5402277f0cfd4e9ac2bf9c0c0cd8e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7af5402277f0cfd4e9ac2bf9c0c0cd8e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b413e4e18e70b2b1bddb54358fbf507e.jpg\" _src=\"http://yanxuan.nosdn.127.net/b413e4e18e70b2b1bddb54358fbf507e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2006d2a3ff91300d1265ce875433484a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2006d2a3ff91300d1265ce875433484a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35c5c281c7b8bfe5a67704abfbd0f550.jpg\" _src=\"http://yanxuan.nosdn.127.net/35c5c281c7b8bfe5a67704abfbd0f550.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f30d0dd64c48d72f543cf7f48f66f48.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f30d0dd64c48d72f543cf7f48f66f48.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/13632b105431e683733b69d8a065d458.jpg\" _src=\"http://yanxuan.nosdn.127.net/13632b105431e683733b69d8a065d458.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3a10c77b61704c1efa426d566ead340.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3a10c77b61704c1efa426d566ead340.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 22,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/eb9fd89dcabcbcf7ed7b86a3cb47c96e.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/cc45baafad00405699552c187c64c512.png",
      "retail_price": 49,
      "sell_volume": 997,
      "primary_product_id": 1085010,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1081002,
      "category_id": 1008002,
      "goods_sn": "1081002",
      "name": "北欧风珊瑚绒多功能抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "靠枕暖手毛毯多用",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/d3afdc4dc4f7e8700abd3befd8786f9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3afdc4dc4f7e8700abd3befd8786f9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/690e4238d3c6fe734e5a5a8e5d567cf2.jpg\" _src=\"http://yanxuan.nosdn.127.net/690e4238d3c6fe734e5a5a8e5d567cf2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3bb465550fcf6bafcde2b11b4a96d799.jpg\" _src=\"http://yanxuan.nosdn.127.net/3bb465550fcf6bafcde2b11b4a96d799.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b4ba8661f77ff02edc7a172ea1489a3.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b4ba8661f77ff02edc7a172ea1489a3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ededcff020a14eecad669b5beeba3f30.jpg\" _src=\"http://yanxuan.nosdn.127.net/ededcff020a14eecad669b5beeba3f30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/394992289ec493441e7e91dd8a6e856b.jpg\" _src=\"http://yanxuan.nosdn.127.net/394992289ec493441e7e91dd8a6e856b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f06eb02e8ed368a868dfd8137d1c7f3b.jpg\" _src=\"http://yanxuan.nosdn.127.net/f06eb02e8ed368a868dfd8137d1c7f3b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cec7fcfda67bf3ed1ee66e887614d633.jpg\" _src=\"http://yanxuan.nosdn.127.net/cec7fcfda67bf3ed1ee66e887614d633.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19ffcfd2a998820e92656611ba6ccd99.jpg\" _src=\"http://yanxuan.nosdn.127.net/19ffcfd2a998820e92656611ba6ccd99.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c698e643a9ababb498f36b2dd948f59.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c698e643a9ababb498f36b2dd948f59.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9746e6314f6aec06be56e6b1f54972c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9746e6314f6aec06be56e6b1f54972c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/769eee41f1452888fa632c07551ca400.jpg\" _src=\"http://yanxuan.nosdn.127.net/769eee41f1452888fa632c07551ca400.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65c740031e1cd5792aecc6333710fe06.jpg\" _src=\"http://yanxuan.nosdn.127.net/65c740031e1cd5792aecc6333710fe06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/42361e27db7a3b76705568c0f57bfd43.jpg\" _src=\"http://yanxuan.nosdn.127.net/42361e27db7a3b76705568c0f57bfd43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8a3048b4a8ea13487faa1ff51c394ad3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8a3048b4a8ea13487faa1ff51c394ad3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/032041aaae3d703194d7fab7599c4495.jpg\" _src=\"http://yanxuan.nosdn.127.net/032041aaae3d703194d7fab7599c4495.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2478a21152ad10d517af58aaaed64214.jpg\" _src=\"http://yanxuan.nosdn.127.net/2478a21152ad10d517af58aaaed64214.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92691014c72fd7f34f6fada58162011f.jpg\" _src=\"http://yanxuan.nosdn.127.net/92691014c72fd7f34f6fada58162011f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9dc547b23d58f4a835008b55f797f4bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/9dc547b23d58f4a835008b55f797f4bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf6a80f009ba96e51851dce228e542b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf6a80f009ba96e51851dce228e542b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52674285cdb5d2ea19967d3188d1ff8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/52674285cdb5d2ea19967d3188d1ff8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eeb3c5128f915416f4b60a968230d320.jpg\" _src=\"http://yanxuan.nosdn.127.net/eeb3c5128f915416f4b60a968230d320.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/998cc7acd5ce1797aa4b32f8ef775148.jpg\" _src=\"http://yanxuan.nosdn.127.net/998cc7acd5ce1797aa4b32f8ef775148.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d7d12038de9483c3974c3ad8f20927a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/d7d12038de9483c3974c3ad8f20927a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f3c6b9f3fdf0c48156251636e513720e.jpg\" _src=\"http://yanxuan.nosdn.127.net/f3c6b9f3fdf0c48156251636e513720e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/367b80cefe0803348720f82f1c30cfe7.jpg\" _src=\"http://yanxuan.nosdn.127.net/367b80cefe0803348720f82f1c30cfe7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c360e0a65e58cc1c04e01eed6f04b54b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c360e0a65e58cc1c04e01eed6f04b54b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6e60d12aff676400bad21d0c93b67803.jpg\" _src=\"http://yanxuan.nosdn.127.net/6e60d12aff676400bad21d0c93b67803.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8be1fb462d145316ec2264d5025b8a48.jpg\" _src=\"http://yanxuan.nosdn.127.net/8be1fb462d145316ec2264d5025b8a48.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80725f3251d122a8bc66b20814648310.jpg\" _src=\"http://yanxuan.nosdn.127.net/80725f3251d122a8bc66b20814648310.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a6a82ed8c28b0c60b45bb38e4e7ce04.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a6a82ed8c28b0c60b45bb38e4e7ce04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae881c80e00c34e59c7fd77f829b9931.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae881c80e00c34e59c7fd77f829b9931.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10d7b57b8772053d38fca8e7f6856bac.jpg\" _src=\"http://yanxuan.nosdn.127.net/10d7b57b8772053d38fca8e7f6856bac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6d43e30b2aaac4a81dec473fc2842984.jpg\" _src=\"http://yanxuan.nosdn.127.net/6d43e30b2aaac4a81dec473fc2842984.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdd8426becc5a730730838e264c8c998.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdd8426becc5a730730838e264c8c998.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2aaf853063048b8485c1219b8ba55ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2aaf853063048b8485c1219b8ba55ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70604ff736ccc200037d247a274ac128.jpg\" _src=\"http://yanxuan.nosdn.127.net/70604ff736ccc200037d247a274ac128.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3778c8814cba4fa56d697d6e7c84e5dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/3778c8814cba4fa56d697d6e7c84e5dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa66cda001dd6ba7281f9808da9a344b.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa66cda001dd6ba7281f9808da9a344b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65955a09afe2dfa08a92e3b70bda0f5d.jpg\" _src=\"http://yanxuan.nosdn.127.net/65955a09afe2dfa08a92e3b70bda0f5d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/46bd1859ec91d296d8367e2e6a97ec11.jpg\" _src=\"http://yanxuan.nosdn.127.net/46bd1859ec91d296d8367e2e6a97ec11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33259dcc01613bbf0bb8313f9129e7bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/33259dcc01613bbf0bb8313f9129e7bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5fa03cc2c17cc38da8dc84d0c0e42fa2.jpg\" _src=\"http://yanxuan.nosdn.127.net/5fa03cc2c17cc38da8dc84d0c0e42fa2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5baa2bc5c725dd3d8522b7766830bcb.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5baa2bc5c725dd3d8522b7766830bcb.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 21,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/b87b4b80910fa03b92923997fd4aabd9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/380cfcd5d8bc22360de089f0b4eb11da.png",
      "retail_price": 89,
      "sell_volume": 132,
      "primary_product_id": 1085012,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 1
    },
    {
      "id": 1115052,
      "category_id": 1008002,
      "goods_sn": "1115052",
      "name": "日式和风蔺草蒲团坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "龙眉蔺草编织 日式茶禅风",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/c5c39ed4982045a32efde6f8e4b3d327.jpg\" _src=\"http://yanxuan.nosdn.127.net/c5c39ed4982045a32efde6f8e4b3d327.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/385b1a317b993c403f5b1532bf714592.jpg\" _src=\"http://yanxuan.nosdn.127.net/385b1a317b993c403f5b1532bf714592.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97c44d5c2411a2b8bb39ee34957783bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/97c44d5c2411a2b8bb39ee34957783bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/489a326e13a5bb3ce44a40fc71ccbc40.jpg\" _src=\"http://yanxuan.nosdn.127.net/489a326e13a5bb3ce44a40fc71ccbc40.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2d6eb8e6ba1de0db4bdc1d4ef8d124d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2d6eb8e6ba1de0db4bdc1d4ef8d124d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e723ef50260b98666955796f6dab4c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e723ef50260b98666955796f6dab4c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3cd9585a68c6b746f509408c2c16783a.jpg\" _src=\"http://yanxuan.nosdn.127.net/3cd9585a68c6b746f509408c2c16783a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/582bdb6e01ad3b8f2d76d0124dfdcf8e.jpg\" _src=\"http://yanxuan.nosdn.127.net/582bdb6e01ad3b8f2d76d0124dfdcf8e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8dd281a87afd1ae88dc05e1db35142a4.jpg\" _src=\"http://yanxuan.nosdn.127.net/8dd281a87afd1ae88dc05e1db35142a4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/73a608d337ac09b75b4bd14d8170b6d6.jpg\" _src=\"http://yanxuan.nosdn.127.net/73a608d337ac09b75b4bd14d8170b6d6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fdc10bae153b0dda81dd53b57c2b9e10.jpg\" _src=\"http://yanxuan.nosdn.127.net/fdc10bae153b0dda81dd53b57c2b9e10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cccdb8b1831f0b70306a4b4eed8859db.jpg\" _src=\"http://yanxuan.nosdn.127.net/cccdb8b1831f0b70306a4b4eed8859db.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5baf78b4175b0fdb0132b5d83bb7e279.jpg\" _src=\"http://yanxuan.nosdn.127.net/5baf78b4175b0fdb0132b5d83bb7e279.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e613832e2b3e0cfcad1c42e6cf3d6d3e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e613832e2b3e0cfcad1c42e6cf3d6d3e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de9c7cedfd555ceb5adfed1c0c96b9b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/de9c7cedfd555ceb5adfed1c0c96b9b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61a0ecae290671c15ac857e0f5b8fb5f.jpg\" _src=\"http://yanxuan.nosdn.127.net/61a0ecae290671c15ac857e0f5b8fb5f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8f15359576d133d55457f69c05aeab8.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8f15359576d133d55457f69c05aeab8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aae2ff89028e265b06656aa63a94c58e.jpg\" _src=\"http://yanxuan.nosdn.127.net/aae2ff89028e265b06656aa63a94c58e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbecb94e2a020007505cad42c4e8553a.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbecb94e2a020007505cad42c4e8553a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4adb8529010d4348b90cdc445f37d241.jpg\" _src=\"http://yanxuan.nosdn.127.net/4adb8529010d4348b90cdc445f37d241.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/953207acdb90210c681deb18b59fdadb.jpg\" _src=\"http://yanxuan.nosdn.127.net/953207acdb90210c681deb18b59fdadb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa5b73dea7f39614c01de4ee8acdc216.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa5b73dea7f39614c01de4ee8acdc216.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2b7ccd3a548618f2fadb20aee9ab9531.jpg\" _src=\"http://yanxuan.nosdn.127.net/2b7ccd3a548618f2fadb20aee9ab9531.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ecde950588789c70df2222f1ded0f579.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecde950588789c70df2222f1ded0f579.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/597505ee5976bf7f68646ef2321c5b39.jpg\" _src=\"http://yanxuan.nosdn.127.net/597505ee5976bf7f68646ef2321c5b39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f317d788383403a224a191452183b9f.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f317d788383403a224a191452183b9f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ca568894e24f4aa5d6eaf4174667ffa.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ca568894e24f4aa5d6eaf4174667ffa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdbf86365486d602bc2c2b1aa4bd8781.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdbf86365486d602bc2c2b1aa4bd8781.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa9db3d211c93fa9d2914754464e679c.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa9db3d211c93fa9d2914754464e679c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/58e5cd852682d404200f57471e883485.jpg\" _src=\"http://yanxuan.nosdn.127.net/58e5cd852682d404200f57471e883485.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14cc6189a160dcf8f0d2f0d0bd0b7f27.jpg\" _src=\"http://yanxuan.nosdn.127.net/14cc6189a160dcf8f0d2f0d0bd0b7f27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c49b33afea38804de07fc9a6bb80dda9.jpg\" _src=\"http://yanxuan.nosdn.127.net/c49b33afea38804de07fc9a6bb80dda9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8cf4bc3c1b476cba2ec6290b02c698be.jpg\" _src=\"http://yanxuan.nosdn.127.net/8cf4bc3c1b476cba2ec6290b02c698be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3d5eb1291c79204e2e23dede15b8cac.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3d5eb1291c79204e2e23dede15b8cac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38791f147ef4ee52bfee5e240f2a5f52.jpg\" _src=\"http://yanxuan.nosdn.127.net/38791f147ef4ee52bfee5e240f2a5f52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9756648996576857cabe3740da2edaa6.jpg\" _src=\"http://yanxuan.nosdn.127.net/9756648996576857cabe3740da2edaa6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f4247a5ccb0f39be52a8c99cb15f92f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/f4247a5ccb0f39be52a8c99cb15f92f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40d0ceae7b2300246501b72540727505.jpg\" _src=\"http://yanxuan.nosdn.127.net/40d0ceae7b2300246501b72540727505.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14603e5d6e54d7e1abaae04ea713de08.jpg\" _src=\"http://yanxuan.nosdn.127.net/14603e5d6e54d7e1abaae04ea713de08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/06d66618b49e447645e3650dc6cb11ca.jpg\" _src=\"http://yanxuan.nosdn.127.net/06d66618b49e447645e3650dc6cb11ca.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ef12ad1adb0d16743a0054489846a13.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ef12ad1adb0d16743a0054489846a13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99d648a6665d2a25f790a469c464d34b.jpg\" _src=\"http://yanxuan.nosdn.127.net/99d648a6665d2a25f790a469c464d34b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76e121103fb90fdf267eb204af59c0d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/76e121103fb90fdf267eb204af59c0d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9d92a1874c26534262643772dbdef1d2.jpg\" _src=\"http://yanxuan.nosdn.127.net/9d92a1874c26534262643772dbdef1d2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cb04ad36ddc0b45066f8233ab9cf888.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cb04ad36ddc0b45066f8233ab9cf888.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cdb4947e9c035fea2bb271c9f0b43d2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/cdb4947e9c035fea2bb271c9f0b43d2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55c1446b40d52e2da86f92fccc47ea2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/55c1446b40d52e2da86f92fccc47ea2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/339c0d5acef5c3029fd3c0d500883ce5.jpg\" _src=\"http://yanxuan.nosdn.127.net/339c0d5acef5c3029fd3c0d500883ce5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11dc59302185026721eaa23509c333ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/11dc59302185026721eaa23509c333ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/81ed48a7099d3bfa9860fcdd4e546b60.jpg\" _src=\"http://yanxuan.nosdn.127.net/81ed48a7099d3bfa9860fcdd4e546b60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c615061f6c675ba67897e03e1f9cee17.jpg\" _src=\"http://yanxuan.nosdn.127.net/c615061f6c675ba67897e03e1f9cee17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e30a5c3df143363971c97e75f254818d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e30a5c3df143363971c97e75f254818d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b33a8b54250cf02206d1d9fa5674725.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b33a8b54250cf02206d1d9fa5674725.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf292ce53420b314368494c36b189ce1.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf292ce53420b314368494c36b189ce1.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 18,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/66d736aa8e3e33e3c76a014e1379c9a9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/39dea35a3ea2361e4b054ee2f421af53.png",
      "retail_price": 86,
      "sell_volume": 5586,
      "primary_product_id": 1116105,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1128002,
      "category_id": 1008002,
      "goods_sn": "1128002",
      "name": "清新趣粉系列居家地毯 青粉拼接",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "清新撞色 细腻柔软",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/191b701367615b452976b4c740ef1c52.jpg\" _src=\"http://yanxuan.nosdn.127.net/191b701367615b452976b4c740ef1c52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f83f2a2b556d9d0b4b4a65ca76f4689.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f83f2a2b556d9d0b4b4a65ca76f4689.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/119231f5f75494b2249cd14009b452aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/119231f5f75494b2249cd14009b452aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/085c0b2b140f9b3e499209f3ca2b3b16.jpg\" _src=\"http://yanxuan.nosdn.127.net/085c0b2b140f9b3e499209f3ca2b3b16.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ac2cdba24df037dfe0704bd47c73d3e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/ac2cdba24df037dfe0704bd47c73d3e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35def50dabd355332d47a994e29a53c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/35def50dabd355332d47a994e29a53c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0378678601a27aa2e0fea8fcd757ae51.jpg\" _src=\"http://yanxuan.nosdn.127.net/0378678601a27aa2e0fea8fcd757ae51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c3d214fea7c5a768c7a0f77172a70d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c3d214fea7c5a768c7a0f77172a70d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bec41337e525e74998290e7378f3bb8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bec41337e525e74998290e7378f3bb8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d5d50c46c26a0c2be14d2c845a4e15c5.jpg\" _src=\"http://yanxuan.nosdn.127.net/d5d50c46c26a0c2be14d2c845a4e15c5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c138155947879f4af0e7ce3c7d4713d.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c138155947879f4af0e7ce3c7d4713d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da7c0824e22218d320719560989d537e.jpg\" _src=\"http://yanxuan.nosdn.127.net/da7c0824e22218d320719560989d537e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bf35a5b2a1747108cb8d225f0da227d.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bf35a5b2a1747108cb8d225f0da227d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e93c3ee67c2f953fae54295b0f4a7173.jpg\" _src=\"http://yanxuan.nosdn.127.net/e93c3ee67c2f953fae54295b0f4a7173.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa47796942f2ba1f6bf0032fe316ac27.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa47796942f2ba1f6bf0032fe316ac27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f116e257387af4f48bf2ddb8c840132.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f116e257387af4f48bf2ddb8c840132.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a756a78742cd1e018a66e40e0cf3f5ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/a756a78742cd1e018a66e40e0cf3f5ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/567a0391d29b41c75216203f0327360d.jpg\" _src=\"http://yanxuan.nosdn.127.net/567a0391d29b41c75216203f0327360d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e3bb469a99952ad770a1782ebabe0a3.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e3bb469a99952ad770a1782ebabe0a3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/98e4edc31d260fcfdff9d74527a36361.jpg\" _src=\"http://yanxuan.nosdn.127.net/98e4edc31d260fcfdff9d74527a36361.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8f9871f90756a1833bea06961285087.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8f9871f90756a1833bea06961285087.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa9d442de4aa9b93b48fefafe0f869b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa9d442de4aa9b93b48fefafe0f869b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8c3c00ea6a2f13c5ce37b6dec024edf5.jpg\" _src=\"http://yanxuan.nosdn.127.net/8c3c00ea6a2f13c5ce37b6dec024edf5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d83a1dc525bb6aa23d456efd5a2c74c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d83a1dc525bb6aa23d456efd5a2c74c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7397347cfc3d7ce697386941201d1615.jpg\" _src=\"http://yanxuan.nosdn.127.net/7397347cfc3d7ce697386941201d1615.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e40e07ef01e1950ddb708d6ed56eea3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e40e07ef01e1950ddb708d6ed56eea3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb59b7f4df5d97e9ac407fe75e095e81.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb59b7f4df5d97e9ac407fe75e095e81.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6660e07c91870230941f9bfe160f9f49.jpg\" _src=\"http://yanxuan.nosdn.127.net/6660e07c91870230941f9bfe160f9f49.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e40bb0099d592ca0f1335eabe43570cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/e40bb0099d592ca0f1335eabe43570cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7310efd4551e1a851668d01733711d39.jpg\" _src=\"http://yanxuan.nosdn.127.net/7310efd4551e1a851668d01733711d39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c7ab57bdf16a7a88e526e82deba2879.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c7ab57bdf16a7a88e526e82deba2879.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e1a120dc4898e9e871d4005d30c7937.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e1a120dc4898e9e871d4005d30c7937.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22fe678cf2b8e594c15fba60f86b717e.jpg\" _src=\"http://yanxuan.nosdn.127.net/22fe678cf2b8e594c15fba60f86b717e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c7e4053e6340d8fc377babc65cd40823.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7e4053e6340d8fc377babc65cd40823.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ae576390b96e274b10c71104e210d33.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ae576390b96e274b10c71104e210d33.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/425feec1ad943958c28edaf1504af645.jpg\" _src=\"http://yanxuan.nosdn.127.net/425feec1ad943958c28edaf1504af645.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e8d1bd0e0277e74509d074f2a931f1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e8d1bd0e0277e74509d074f2a931f1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e67f6b3d18df8ddf931b4468f35d4fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e67f6b3d18df8ddf931b4468f35d4fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33951c6621e5b91ee1c1b9958f9bb57a.jpg\" _src=\"http://yanxuan.nosdn.127.net/33951c6621e5b91ee1c1b9958f9bb57a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e80772f6663a57de51494fec4369524b.jpg\" _src=\"http://yanxuan.nosdn.127.net/e80772f6663a57de51494fec4369524b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e2516cafe760408782a8427a5015b98.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e2516cafe760408782a8427a5015b98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2fe4275c5b83193c1562e2f5dbf72442.jpg\" _src=\"http://yanxuan.nosdn.127.net/2fe4275c5b83193c1562e2f5dbf72442.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1d4aa2f956ef90e826b50cb16db731a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1d4aa2f956ef90e826b50cb16db731a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c9afc1b180779690891a23e9adb2265.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c9afc1b180779690891a23e9adb2265.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d4323b01083e2aa3eec9e28402b612b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d4323b01083e2aa3eec9e28402b612b.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 27,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/dbf282e81ab8b0dbc4b4ad1f4fd6d1e3.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/a1094a808ffb3a52a6cb13565a283d98.png",
      "retail_price": 599,
      "sell_volume": 137,
      "primary_product_id": 1128017,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1130037,
      "category_id": 1008002,
      "goods_sn": "1130037",
      "name": "帆布丝羽绒多用坐垫",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "柔软蓬松，透气防螨。",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/96eb609f4f459ab9c502eca7d6e7e204.jpg\" _src=\"http://yanxuan.nosdn.127.net/96eb609f4f459ab9c502eca7d6e7e204.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a86dcf95f3a56db6b7f99f35585dbf2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a86dcf95f3a56db6b7f99f35585dbf2d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bced9d39bcb740a4655ce725f4823e96.jpg\" _src=\"http://yanxuan.nosdn.127.net/bced9d39bcb740a4655ce725f4823e96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11213e448a23292458adc934a643c076.jpg\" _src=\"http://yanxuan.nosdn.127.net/11213e448a23292458adc934a643c076.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9116d858fd59f1ed32fc8a692dfc3fed.jpg\" _src=\"http://yanxuan.nosdn.127.net/9116d858fd59f1ed32fc8a692dfc3fed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b5982e9a43ccaa724f397c9e777b026.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b5982e9a43ccaa724f397c9e777b026.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e4397bee1cf9589eaaf06b8fe9d0a778.jpg\" _src=\"http://yanxuan.nosdn.127.net/e4397bee1cf9589eaaf06b8fe9d0a778.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/740affd3cef0ef40378c2cb265322f15.jpg\" _src=\"http://yanxuan.nosdn.127.net/740affd3cef0ef40378c2cb265322f15.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6aeacc205ef12e2a475eb7a8e8d1eedc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6aeacc205ef12e2a475eb7a8e8d1eedc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/119709a17d08f2c1c48d95d24b34ca3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/119709a17d08f2c1c48d95d24b34ca3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8332210d4b81d04f42612fc097db259a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8332210d4b81d04f42612fc097db259a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be1775926acb0e26b6012cba7893e979.jpg\" _src=\"http://yanxuan.nosdn.127.net/be1775926acb0e26b6012cba7893e979.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c6463b2f53c89273f1f79b22dd9e399.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c6463b2f53c89273f1f79b22dd9e399.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38ad3258ebf23df5164854fe403d1ecf.jpg\" _src=\"http://yanxuan.nosdn.127.net/38ad3258ebf23df5164854fe403d1ecf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dc5f238dcb73c249f813233d81156c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dc5f238dcb73c249f813233d81156c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb132e2e8a254b8cbc345900f6fe3c39.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb132e2e8a254b8cbc345900f6fe3c39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0603f40fefd14ee24e83102c5f09100a.jpg\" _src=\"http://yanxuan.nosdn.127.net/0603f40fefd14ee24e83102c5f09100a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/45966f38135adc1280a667040d8e02c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/45966f38135adc1280a667040d8e02c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1064a54404b6c795eae261334697e050.jpg\" _src=\"http://yanxuan.nosdn.127.net/1064a54404b6c795eae261334697e050.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ef89417a81ac1893c95179585bf1140.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ef89417a81ac1893c95179585bf1140.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c2cd2da4d75a63ada7c655e53c223a0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/c2cd2da4d75a63ada7c655e53c223a0e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e942519448a5de394885730e0e3e4694.jpg\" _src=\"http://yanxuan.nosdn.127.net/e942519448a5de394885730e0e3e4694.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d016a18c381916813c2eaf46c3f791c1.jpg\" _src=\"http://yanxuan.nosdn.127.net/d016a18c381916813c2eaf46c3f791c1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6935f94bc80c11c89c3f8a2aa02c4273.jpg\" _src=\"http://yanxuan.nosdn.127.net/6935f94bc80c11c89c3f8a2aa02c4273.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9dedb80199b09770b98fa46cd8a8752d.jpg\" _src=\"http://yanxuan.nosdn.127.net/9dedb80199b09770b98fa46cd8a8752d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f447537304e43a44b1e75272d3334899.jpg\" _src=\"http://yanxuan.nosdn.127.net/f447537304e43a44b1e75272d3334899.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10d901511a3d5f03be68bd64dbadfe1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/10d901511a3d5f03be68bd64dbadfe1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b03a90f7bb697a9bc6e0be9d9997b11.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b03a90f7bb697a9bc6e0be9d9997b11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62b277f50e7cca075cd2565a4f2b4466.jpg\" _src=\"http://yanxuan.nosdn.127.net/62b277f50e7cca075cd2565a4f2b4466.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e304f8f1ea10792be9072d3c7a4a8359.jpg\" _src=\"http://yanxuan.nosdn.127.net/e304f8f1ea10792be9072d3c7a4a8359.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d7c39350bee7fdc8bdb78a27eb83a17.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d7c39350bee7fdc8bdb78a27eb83a17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/742927f31cadc641a7b9bb3fc5eebfe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/742927f31cadc641a7b9bb3fc5eebfe3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2562d7d1a0fa4b9497e4ec719f08a8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2562d7d1a0fa4b9497e4ec719f08a8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/430442f4524e66347fbbf10aaf213a07.jpg\" _src=\"http://yanxuan.nosdn.127.net/430442f4524e66347fbbf10aaf213a07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/620ec1f6387fa84f5518ad2484ebaa91.jpg\" _src=\"http://yanxuan.nosdn.127.net/620ec1f6387fa84f5518ad2484ebaa91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/455f215b9a402ed9c0c0972c0abddbb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/455f215b9a402ed9c0c0972c0abddbb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1def5c3403bdf5cd7e11b85354542452.jpg\" _src=\"http://yanxuan.nosdn.127.net/1def5c3403bdf5cd7e11b85354542452.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97348238ae3c27a56ff46e1b6c3deb3b.jpg\" _src=\"http://yanxuan.nosdn.127.net/97348238ae3c27a56ff46e1b6c3deb3b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3739461a5eb338a70e7d34a86ff26d1a.jpg\" _src=\"http://yanxuan.nosdn.127.net/3739461a5eb338a70e7d34a86ff26d1a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/96fae2f2cc374d459c3969e7a7cc1a83.jpg\" _src=\"http://yanxuan.nosdn.127.net/96fae2f2cc374d459c3969e7a7cc1a83.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c1654fc509c8c77e9fe4c75ffc099f24.jpg\" _src=\"http://yanxuan.nosdn.127.net/c1654fc509c8c77e9fe4c75ffc099f24.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf95ab8945e61c7180eba1e01721b15a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf95ab8945e61c7180eba1e01721b15a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b054e088382a0cb32a529082c52745e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b054e088382a0cb32a529082c52745e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d517d1ca7532cde5cc74ad2a10dc17.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d517d1ca7532cde5cc74ad2a10dc17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6222e1fd9b42422e8454cc087a0e0358.jpg\" _src=\"http://yanxuan.nosdn.127.net/6222e1fd9b42422e8454cc087a0e0358.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8995022af1826e846b7a143e7b8b325.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8995022af1826e846b7a143e7b8b325.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a12c940956234db2f60a2b5b51d6a35.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a12c940956234db2f60a2b5b51d6a35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4be7d3058e6eec27a4be033642359535.jpg\" _src=\"http://yanxuan.nosdn.127.net/4be7d3058e6eec27a4be033642359535.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2eca2f02d4ec269cc1893876fb17511a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2eca2f02d4ec269cc1893876fb17511a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf761716e3b430f63e059a891703200e.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf761716e3b430f63e059a891703200e.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 17,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2d1f51656c0bff4989e43b17b42f7ad9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/19ecd7c6f6f31219cf75117238d95139.png",
      "retail_price": 39,
      "sell_volume": 9661,
      "primary_product_id": 1130120,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1130041,
      "category_id": 1008002,
      "goods_sn": "1130041",
      "name": "皮毛一体多用长毛坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "澳洲羊毛的细腻触感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/a83b7218bebd4a83c0b9f6f8a5ea6d08.jpg\" _src=\"http://yanxuan.nosdn.127.net/a83b7218bebd4a83c0b9f6f8a5ea6d08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7eb4d058e83cd9b6aadf5c20c63bcb1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7eb4d058e83cd9b6aadf5c20c63bcb1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/731f44716c3c585f563196c887544f52.jpg\" _src=\"http://yanxuan.nosdn.127.net/731f44716c3c585f563196c887544f52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59afb77cc310a6fde3eabd6401e8bab1.jpg\" _src=\"http://yanxuan.nosdn.127.net/59afb77cc310a6fde3eabd6401e8bab1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db3c78a5adad2a0ea8d219083e8547b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/db3c78a5adad2a0ea8d219083e8547b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/267cc4ac41d6632aec5b18e2026739dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/267cc4ac41d6632aec5b18e2026739dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76a367af57d38c0bc77086e784c2b1d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/76a367af57d38c0bc77086e784c2b1d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c092b3925ee7b5b7dbea29c528ad8db8.jpg\" _src=\"http://yanxuan.nosdn.127.net/c092b3925ee7b5b7dbea29c528ad8db8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aac2f3d5806016fb150d85bebc93b2e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/aac2f3d5806016fb150d85bebc93b2e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cfeb9a9bfcf4338db92e6d8709aef44.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cfeb9a9bfcf4338db92e6d8709aef44.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/453d3f8a6e61298886c3fa4361b59605.jpg\" _src=\"http://yanxuan.nosdn.127.net/453d3f8a6e61298886c3fa4361b59605.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d25fcc0a95baeba59f30b59afa3ff159.jpg\" _src=\"http://yanxuan.nosdn.127.net/d25fcc0a95baeba59f30b59afa3ff159.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ee00ea5c06c29973db9cf3c499ef0ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ee00ea5c06c29973db9cf3c499ef0ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23c51b8a7d25e88cc510609363f254a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/23c51b8a7d25e88cc510609363f254a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/07a632e4319a4cc45df6404975a4856a.jpg\" _src=\"http://yanxuan.nosdn.127.net/07a632e4319a4cc45df6404975a4856a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f20bda3dd2f724c3871226efc8ab3e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f20bda3dd2f724c3871226efc8ab3e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e237eaaad9484fa1ab1f4a8050df712.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e237eaaad9484fa1ab1f4a8050df712.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/68be7318cc3708254004b1f25abca889.jpg\" _src=\"http://yanxuan.nosdn.127.net/68be7318cc3708254004b1f25abca889.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c0aabf924bbb70486bb38bdf0fe0b9ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/c0aabf924bbb70486bb38bdf0fe0b9ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/938abacde4b46e5fce40c8cb6b5a31f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/938abacde4b46e5fce40c8cb6b5a31f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/560dc26811c85df2a81425ccc80f2daf.jpg\" _src=\"http://yanxuan.nosdn.127.net/560dc26811c85df2a81425ccc80f2daf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ea86c3ab570b110f24322dc88a2bf67c.jpg\" _src=\"http://yanxuan.nosdn.127.net/ea86c3ab570b110f24322dc88a2bf67c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20b35a848e5b3e68039d8825ebaf0a92.jpg\" _src=\"http://yanxuan.nosdn.127.net/20b35a848e5b3e68039d8825ebaf0a92.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/613568156bb735d4e826fadf9b14f30a.jpg\" _src=\"http://yanxuan.nosdn.127.net/613568156bb735d4e826fadf9b14f30a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c2626064e1a840a3fd0d8937092a2a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c2626064e1a840a3fd0d8937092a2a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4710cebed0fec2581f6c9d7a0ad35f4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4710cebed0fec2581f6c9d7a0ad35f4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab23943bde5aee5a2f4db6305a638d06.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab23943bde5aee5a2f4db6305a638d06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f1722c1d44e6791a239d20ae2a84cb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f1722c1d44e6791a239d20ae2a84cb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec18f626b235961bba578d8726ab5d80.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec18f626b235961bba578d8726ab5d80.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7c162a729f465edd62b2489af405820.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7c162a729f465edd62b2489af405820.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de81035e3a2a44ad0420d25b374b248a.jpg\" _src=\"http://yanxuan.nosdn.127.net/de81035e3a2a44ad0420d25b374b248a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92fcfcee4d8a828fcbda97ecd4ac7c61.jpg\" _src=\"http://yanxuan.nosdn.127.net/92fcfcee4d8a828fcbda97ecd4ac7c61.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c98e8d8abc2f97df7fa1ed3e8a19e793.jpg\" _src=\"http://yanxuan.nosdn.127.net/c98e8d8abc2f97df7fa1ed3e8a19e793.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/505355f028aafae9ac04ef604c46a89d.jpg\" _src=\"http://yanxuan.nosdn.127.net/505355f028aafae9ac04ef604c46a89d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3439e5f1fce7f602ae8fabce64e3bafa.jpg\" _src=\"http://yanxuan.nosdn.127.net/3439e5f1fce7f602ae8fabce64e3bafa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2ceea236ef9f0b2198dfce82e9265c06.jpg\" _src=\"http://yanxuan.nosdn.127.net/2ceea236ef9f0b2198dfce82e9265c06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/784fe3f5f7fdeebdb26b2dab8542d1f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/784fe3f5f7fdeebdb26b2dab8542d1f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15e4f99d5d272b0680868d2007d64382.jpg\" _src=\"http://yanxuan.nosdn.127.net/15e4f99d5d272b0680868d2007d64382.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99c09fe7b0d3ca49a81c7df0cc0a9dc1.jpg\" _src=\"http://yanxuan.nosdn.127.net/99c09fe7b0d3ca49a81c7df0cc0a9dc1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65c12643b55584e3e0474292c42088ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/65c12643b55584e3e0474292c42088ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d8d75b4b195d6086a44f2ee6d906d12.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d8d75b4b195d6086a44f2ee6d906d12.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c52456cd1b25174f0222273b7394a5b7.jpg\" _src=\"http://yanxuan.nosdn.127.net/c52456cd1b25174f0222273b7394a5b7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a089ad7a18777861c80d185b090dedc9.jpg\" _src=\"http://yanxuan.nosdn.127.net/a089ad7a18777861c80d185b090dedc9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/671ddba19da9b13492dbb5e3126fc018.jpg\" _src=\"http://yanxuan.nosdn.127.net/671ddba19da9b13492dbb5e3126fc018.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f60ed6e112c17e1ddbb301181477e8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f60ed6e112c17e1ddbb301181477e8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2a5a06bac71ceb645b47a322bef9588.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2a5a06bac71ceb645b47a322bef9588.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f612db88ffb6d1b7287039c8d3aee82d.jpg\" _src=\"http://yanxuan.nosdn.127.net/f612db88ffb6d1b7287039c8d3aee82d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27daed7f1faba0f42c1b0987eca43e1a.jpg\" _src=\"http://yanxuan.nosdn.127.net/27daed7f1faba0f42c1b0987eca43e1a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20a180e85c13f5ece01875ad91842193.jpg\" _src=\"http://yanxuan.nosdn.127.net/20a180e85c13f5ece01875ad91842193.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d42ca472ca07af1e8037673a2d1159e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d42ca472ca07af1e8037673a2d1159e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b161c4bf4b6937ed473449b21c61b8c.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b161c4bf4b6937ed473449b21c61b8c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76b268744bf751b5783ada179c343474.jpg\" _src=\"http://yanxuan.nosdn.127.net/76b268744bf751b5783ada179c343474.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18606e0a3c59f2a26585fbdd6a5dcedd.jpg\" _src=\"http://yanxuan.nosdn.127.net/18606e0a3c59f2a26585fbdd6a5dcedd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8636692d4819117b12b27f77506562d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/8636692d4819117b12b27f77506562d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b8d7e96b6cf7fc8dd7a4b9136c9c9c37.jpg\" _src=\"http://yanxuan.nosdn.127.net/b8d7e96b6cf7fc8dd7a4b9136c9c9c37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a69f5909a0ebf3450db5117530fbe339.jpg\" _src=\"http://yanxuan.nosdn.127.net/a69f5909a0ebf3450db5117530fbe339.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/00e9909b758d7585ac99423105b6d4a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/00e9909b758d7585ac99423105b6d4a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2ba5974ae02618ba26ff2bb17f3f13ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/2ba5974ae02618ba26ff2bb17f3f13ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9bea1ce19478453bbbe46607b7a7880c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9bea1ce19478453bbbe46607b7a7880c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec70f25fdeab6b03b4b8f01dc070f5d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec70f25fdeab6b03b4b8f01dc070f5d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50bbfa868ba0fc8d424bf1ec82f78ac6.jpg\" _src=\"http://yanxuan.nosdn.127.net/50bbfa868ba0fc8d424bf1ec82f78ac6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b634157638fba9765dd10caf729e27e0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b634157638fba9765dd10caf729e27e0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79ccb6cc4a76e2b69976d3f279539b94.jpg\" _src=\"http://yanxuan.nosdn.127.net/79ccb6cc4a76e2b69976d3f279539b94.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 19,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a1f9e49a91ffda1505501d5015f30cda.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/442b9d99c0e7f39efd7967e0e5987374.png",
      "retail_price": 109,
      "sell_volume": 4383,
      "primary_product_id": 1130127,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1130042,
      "category_id": 1008002,
      "goods_sn": "1130042",
      "name": "皮毛一体多用单张长毛皮垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "盖毯、沙发垫、椅垫、地垫",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/d4ace79c311683de546aba0830b13cef.jpg\" _src=\"http://yanxuan.nosdn.127.net/d4ace79c311683de546aba0830b13cef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18f00b15f815b2d3b37f2348f51ce341.jpg\" _src=\"http://yanxuan.nosdn.127.net/18f00b15f815b2d3b37f2348f51ce341.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a17fcbf654cc3a60c107555af325f0fe.jpg\" _src=\"http://yanxuan.nosdn.127.net/a17fcbf654cc3a60c107555af325f0fe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6feee80476170267af6d71cdfc0b37dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6feee80476170267af6d71cdfc0b37dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/124b182a0a67835b4200cff8176c2b02.jpg\" _src=\"http://yanxuan.nosdn.127.net/124b182a0a67835b4200cff8176c2b02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd74be4a87738afaa04399b4d6d9a870.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd74be4a87738afaa04399b4d6d9a870.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e556cbed463186c4bd99726067b923af.jpg\" _src=\"http://yanxuan.nosdn.127.net/e556cbed463186c4bd99726067b923af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20688f897c671755758786d3040b5c07.jpg\" _src=\"http://yanxuan.nosdn.127.net/20688f897c671755758786d3040b5c07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/260894bbf0796d65bebe0b8af28b6c95.jpg\" _src=\"http://yanxuan.nosdn.127.net/260894bbf0796d65bebe0b8af28b6c95.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/56c59db0a7a2edb57f79cd4ce4725ebd.jpg\" _src=\"http://yanxuan.nosdn.127.net/56c59db0a7a2edb57f79cd4ce4725ebd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f9abac8c992347562001de711510bb03.jpg\" _src=\"http://yanxuan.nosdn.127.net/f9abac8c992347562001de711510bb03.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dfd5efde1a9607ad69344f3feb07cae.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dfd5efde1a9607ad69344f3feb07cae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5563d9a3bcb3063e35ff0a04ea92e0f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/5563d9a3bcb3063e35ff0a04ea92e0f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7106f4f4495f0c3aea5174855ce2e54b.jpg\" _src=\"http://yanxuan.nosdn.127.net/7106f4f4495f0c3aea5174855ce2e54b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da4e5459ca9ce74f3ed0ff5c696d2893.jpg\" _src=\"http://yanxuan.nosdn.127.net/da4e5459ca9ce74f3ed0ff5c696d2893.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9b673bcc593d748b37a81edea189219.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9b673bcc593d748b37a81edea189219.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a72abb429df56c56bbe23b76f9b75204.jpg\" _src=\"http://yanxuan.nosdn.127.net/a72abb429df56c56bbe23b76f9b75204.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb1ba0a44c42710e55d6237a34d34ed6.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb1ba0a44c42710e55d6237a34d34ed6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/370e417d42332266cc31245eef4e2829.jpg\" _src=\"http://yanxuan.nosdn.127.net/370e417d42332266cc31245eef4e2829.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/604f40c00f0529e948a6f6823fe3f8e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/604f40c00f0529e948a6f6823fe3f8e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9ad179d3795a8ebd43f5c9572ba2164.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9ad179d3795a8ebd43f5c9572ba2164.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2cd302f653917f33d9a2d311599ed4f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2cd302f653917f33d9a2d311599ed4f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da22ec1b12867fb95fd7614a7736f76c.jpg\" _src=\"http://yanxuan.nosdn.127.net/da22ec1b12867fb95fd7614a7736f76c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3671bc562ca4d94dc9b87ad90de08ef3.jpg\" _src=\"http://yanxuan.nosdn.127.net/3671bc562ca4d94dc9b87ad90de08ef3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/884bb79eb13e38ded605375476cc07e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/884bb79eb13e38ded605375476cc07e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f7fb86caeb445cf7eaf060f1df33383.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f7fb86caeb445cf7eaf060f1df33383.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/90680bb4193443696a79af88cc5786a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/90680bb4193443696a79af88cc5786a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff03648c6839c642086a35143a0b5059.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff03648c6839c642086a35143a0b5059.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f276b0dd0ca7fcdb576457a46eae4ff3.jpg\" _src=\"http://yanxuan.nosdn.127.net/f276b0dd0ca7fcdb576457a46eae4ff3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c7ec5147aee4c483754a957969029eb2.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7ec5147aee4c483754a957969029eb2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c26d9ad8701cc643cbfc6f69177791bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/c26d9ad8701cc643cbfc6f69177791bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55f4129b1fbcc20d6a0b9e2362043cb5.jpg\" _src=\"http://yanxuan.nosdn.127.net/55f4129b1fbcc20d6a0b9e2362043cb5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02770843341ed31eabb0ddadc5526c52.jpg\" _src=\"http://yanxuan.nosdn.127.net/02770843341ed31eabb0ddadc5526c52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd815b745f3c22fa4cff373d41943a86.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd815b745f3c22fa4cff373d41943a86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/480e0f3996285f44e368a73e6c5fe47d.jpg\" _src=\"http://yanxuan.nosdn.127.net/480e0f3996285f44e368a73e6c5fe47d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/264ee5efd645ca38168ad3bef5496cc5.jpg\" _src=\"http://yanxuan.nosdn.127.net/264ee5efd645ca38168ad3bef5496cc5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c46826b7d93342f359a818e80ec44765.jpg\" _src=\"http://yanxuan.nosdn.127.net/c46826b7d93342f359a818e80ec44765.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaade386233b7b54edadb80675494918.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaade386233b7b54edadb80675494918.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/848aac16cd9d30ce840deb70389c907b.jpg\" _src=\"http://yanxuan.nosdn.127.net/848aac16cd9d30ce840deb70389c907b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c50458c6772905734ff3e7ca1bce9978.jpg\" _src=\"http://yanxuan.nosdn.127.net/c50458c6772905734ff3e7ca1bce9978.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61834d14a5d1d2b77ac92e1baca558c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/61834d14a5d1d2b77ac92e1baca558c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/56ca8b2bc8f4b5ef00b2f87939a11602.jpg\" _src=\"http://yanxuan.nosdn.127.net/56ca8b2bc8f4b5ef00b2f87939a11602.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cb834323e30c14d86a4c1cc9b84d894.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cb834323e30c14d86a4c1cc9b84d894.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85e5f74e7205a9328209ca25be550598.jpg\" _src=\"http://yanxuan.nosdn.127.net/85e5f74e7205a9328209ca25be550598.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ea202d5a703a4291495f5c0f83bed73.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ea202d5a703a4291495f5c0f83bed73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf7433c7f8a437cf93ef90d1431adb57.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf7433c7f8a437cf93ef90d1431adb57.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbeddf135c0fe1f0ecfae5c6c057ea00.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbeddf135c0fe1f0ecfae5c6c057ea00.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/66b9e3c4986788281dece847560367d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/66b9e3c4986788281dece847560367d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e5d979ede709143d5f0f852855768c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e5d979ede709143d5f0f852855768c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce0a7f7bb447aa5148ecd03a7555c820.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce0a7f7bb447aa5148ecd03a7555c820.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e6b8abe385df7425ade75210724ffcc.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e6b8abe385df7425ade75210724ffcc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb3266c177f530869f44f1eaaf0b2bb7.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb3266c177f530869f44f1eaaf0b2bb7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ced47c9582a9353dc71d668467067b9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ced47c9582a9353dc71d668467067b9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae6270545f82ef2bee47fb0fa3d15e04.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae6270545f82ef2bee47fb0fa3d15e04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75d28b0323f8b9586d0339ab881c4e04.jpg\" _src=\"http://yanxuan.nosdn.127.net/75d28b0323f8b9586d0339ab881c4e04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d7750e85464204a7c57f50689eec1db4.jpg\" _src=\"http://yanxuan.nosdn.127.net/d7750e85464204a7c57f50689eec1db4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/373138262298b9c59e33a7cc3fe2f1e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/373138262298b9c59e33a7cc3fe2f1e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f39bae90e169f4e5417e0be5c66ad4df.jpg\" _src=\"http://yanxuan.nosdn.127.net/f39bae90e169f4e5417e0be5c66ad4df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f16ebd2501372da0d4b3e4e516df3fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f16ebd2501372da0d4b3e4e516df3fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f925d64a68d213867ceafc1211d59250.jpg\" _src=\"http://yanxuan.nosdn.127.net/f925d64a68d213867ceafc1211d59250.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eddd76fef80b87e1cf3a8d7bd6ceee3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/eddd76fef80b87e1cf3a8d7bd6ceee3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b74337d99199c178ff101a912cb37212.jpg\" _src=\"http://yanxuan.nosdn.127.net/b74337d99199c178ff101a912cb37212.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6fc6571f3526af0d9126071bd479e35.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6fc6571f3526af0d9126071bd479e35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d26b83628f5e2b2830fd49b52ba67e70.jpg\" _src=\"http://yanxuan.nosdn.127.net/d26b83628f5e2b2830fd49b52ba67e70.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 20,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/e1d2090771d920c3feb477f07ac0ecb2.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/dc9d09334eb201fe9408ed604e549941.png",
      "retail_price": 239,
      "sell_volume": 4702,
      "primary_product_id": 1130130,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1134022,
      "category_id": 1008002,
      "goods_sn": "1134022",
      "name": "清新趣粉防滑浴垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "清新跃动，舒适脚感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/d68e182e560941e807d33431ad82452e.jpg\" _src=\"http://yanxuan.nosdn.127.net/d68e182e560941e807d33431ad82452e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/758e12cde995bc722cbab81644c29f60.jpg\" _src=\"http://yanxuan.nosdn.127.net/758e12cde995bc722cbab81644c29f60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b2cadfcad57975bc4b8ad4cb53ebbad.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b2cadfcad57975bc4b8ad4cb53ebbad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4600c0173de7dfa48d2c7d278667312f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4600c0173de7dfa48d2c7d278667312f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e766cfe5d9f6cf74390e37c271c5193.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e766cfe5d9f6cf74390e37c271c5193.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97d7a034074e100db15b1c94f9f4308f.jpg\" _src=\"http://yanxuan.nosdn.127.net/97d7a034074e100db15b1c94f9f4308f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d78fd7ec09228ed93358f187b6c12398.jpg\" _src=\"http://yanxuan.nosdn.127.net/d78fd7ec09228ed93358f187b6c12398.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/00960ca0bd8f388fc52a493f39beac38.jpg\" _src=\"http://yanxuan.nosdn.127.net/00960ca0bd8f388fc52a493f39beac38.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb505efadcd8bb19d88b7ec1d86d5ade.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb505efadcd8bb19d88b7ec1d86d5ade.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/90ebd0a8cdd8a256b36fd26b2717a655.jpg\" _src=\"http://yanxuan.nosdn.127.net/90ebd0a8cdd8a256b36fd26b2717a655.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f391c39a3455577651ea1b2f7bb4832.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f391c39a3455577651ea1b2f7bb4832.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d153c03f2acc1e3062b507c135b309d6.jpg\" _src=\"http://yanxuan.nosdn.127.net/d153c03f2acc1e3062b507c135b309d6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9b6a5e8636dbfaa875b94c0221bf001.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9b6a5e8636dbfaa875b94c0221bf001.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dc971a8f5c766e3dd9f36fdfe6f9afd3.jpg\" _src=\"http://yanxuan.nosdn.127.net/dc971a8f5c766e3dd9f36fdfe6f9afd3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63dd064c791211bda9f0dfcf0bfe0db7.jpg\" _src=\"http://yanxuan.nosdn.127.net/63dd064c791211bda9f0dfcf0bfe0db7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15ecb7b4d9f3142a073eacd5506c0a2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/15ecb7b4d9f3142a073eacd5506c0a2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/278235956b0cd9a3aab8933c63c923c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/278235956b0cd9a3aab8933c63c923c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84bc90dec0c6f6049a79622f7b9ef83c.jpg\" _src=\"http://yanxuan.nosdn.127.net/84bc90dec0c6f6049a79622f7b9ef83c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9707c4a9a76f0432bb7c2d03b72f9582.jpg\" _src=\"http://yanxuan.nosdn.127.net/9707c4a9a76f0432bb7c2d03b72f9582.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3e75d69e0a16177a5b22a07ce0f39f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3e75d69e0a16177a5b22a07ce0f39f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ea585974061d0c9cc858bf5927f79cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ea585974061d0c9cc858bf5927f79cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aab2d28c54f55eddfeffb9fc7dc5e410.jpg\" _src=\"http://yanxuan.nosdn.127.net/aab2d28c54f55eddfeffb9fc7dc5e410.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9500f694389ca250f09b4f60d1be4f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9500f694389ca250f09b4f60d1be4f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8f76b4a92255fdcccd1015476cf05b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8f76b4a92255fdcccd1015476cf05b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2247af207eb3872a7057f0d3dd0a9033.jpg\" _src=\"http://yanxuan.nosdn.127.net/2247af207eb3872a7057f0d3dd0a9033.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5b557985c26db27b73161505ee5d768.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5b557985c26db27b73161505ee5d768.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c16b77cdd7e12a597e2b8508cfc1e3e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/c16b77cdd7e12a597e2b8508cfc1e3e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1cf32a0024e223dd7e3953f642da5f4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1cf32a0024e223dd7e3953f642da5f4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/594dca141f011e7cab4af1f7a19e19f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/594dca141f011e7cab4af1f7a19e19f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a52b1804711993bd96cdc9ca1ffcd10b.jpg\" _src=\"http://yanxuan.nosdn.127.net/a52b1804711993bd96cdc9ca1ffcd10b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/800bf6fc99f89ee6f0f8155fbd9accdb.jpg\" _src=\"http://yanxuan.nosdn.127.net/800bf6fc99f89ee6f0f8155fbd9accdb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55133777a4a7e79c0b13d31a81c077cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/55133777a4a7e79c0b13d31a81c077cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c5a4faf6e647754c6e364dfc4d5cbad.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c5a4faf6e647754c6e364dfc4d5cbad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18792955e7170d770c0f1cd559baee64.jpg\" _src=\"http://yanxuan.nosdn.127.net/18792955e7170d770c0f1cd559baee64.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2113fedc915eca6a7655f77d16f3a620.jpg\" _src=\"http://yanxuan.nosdn.127.net/2113fedc915eca6a7655f77d16f3a620.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4df06a31810e04bc083b71896ce9a326.jpg\" _src=\"http://yanxuan.nosdn.127.net/4df06a31810e04bc083b71896ce9a326.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29ce24ea1f9ba8c078b31aeaded6aa08.jpg\" _src=\"http://yanxuan.nosdn.127.net/29ce24ea1f9ba8c078b31aeaded6aa08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38e3bf328e84f4047a6d5fd4f66ac445.jpg\" _src=\"http://yanxuan.nosdn.127.net/38e3bf328e84f4047a6d5fd4f66ac445.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/956559986a2e62e87e6ba423964cd0f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/956559986a2e62e87e6ba423964cd0f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e79f219a7f9bbb98cbc7120a1699881e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e79f219a7f9bbb98cbc7120a1699881e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88ef1b4cc27eec82cbd38251be88f091.jpg\" _src=\"http://yanxuan.nosdn.127.net/88ef1b4cc27eec82cbd38251be88f091.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7261638f3f3a7287f150a20afdf4b66a.jpg\" _src=\"http://yanxuan.nosdn.127.net/7261638f3f3a7287f150a20afdf4b66a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebe2fcb1f43d47d335f139611bde77f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebe2fcb1f43d47d335f139611bde77f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7a153e2aaff1060fae1fd6ec41fdef9c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7a153e2aaff1060fae1fd6ec41fdef9c.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 31,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/6e79581984d80627916b6e6035e5c6ae.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/a2b7489b4a2b1c09b66464cede4dabd7.png",
      "retail_price": 79,
      "sell_volume": 2166,
      "primary_product_id": 1135125,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1134030,
      "category_id": 1008002,
      "goods_sn": "1134030",
      "name": "简约知性记忆棉坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "慢回弹海绵，时尚设计。",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/3b31b3c57a7d7f42b13711bd1438d555.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b31b3c57a7d7f42b13711bd1438d555.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e92d9bad2a0339a81b47835f5530a358.jpg\" _src=\"http://yanxuan.nosdn.127.net/e92d9bad2a0339a81b47835f5530a358.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/edabc81fa6c7e66fe1698949f3b2b9f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/edabc81fa6c7e66fe1698949f3b2b9f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3444f640ec6ff6d6a8bcc3ce0f28848f.jpg\" _src=\"http://yanxuan.nosdn.127.net/3444f640ec6ff6d6a8bcc3ce0f28848f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/317ebb6f899631d1ed52759c14170a39.jpg\" _src=\"http://yanxuan.nosdn.127.net/317ebb6f899631d1ed52759c14170a39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f17af0ae3d56d482cec4105d390730a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f17af0ae3d56d482cec4105d390730a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/345a9aba507ca86b34c37c29956eeb83.jpg\" _src=\"http://yanxuan.nosdn.127.net/345a9aba507ca86b34c37c29956eeb83.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38b5c26064c4ea16ce3380bd69d2a671.jpg\" _src=\"http://yanxuan.nosdn.127.net/38b5c26064c4ea16ce3380bd69d2a671.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eabf8d6393d65cbd9e2e87c75dfcc066.jpg\" _src=\"http://yanxuan.nosdn.127.net/eabf8d6393d65cbd9e2e87c75dfcc066.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a703c316292e2c4c0b9d6551b25f1856.jpg\" _src=\"http://yanxuan.nosdn.127.net/a703c316292e2c4c0b9d6551b25f1856.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/734765425e21e073844c1c9e062dc35d.jpg\" _src=\"http://yanxuan.nosdn.127.net/734765425e21e073844c1c9e062dc35d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc24974d903f1d0e109482954f1da8e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc24974d903f1d0e109482954f1da8e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da57cdb5646fbff0cf8007f60304c30f.jpg\" _src=\"http://yanxuan.nosdn.127.net/da57cdb5646fbff0cf8007f60304c30f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddc76ceaeddfd7b527df40e01bf7877b.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddc76ceaeddfd7b527df40e01bf7877b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c158fdad4e3c80f90b02cf930b661bb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c158fdad4e3c80f90b02cf930b661bb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9682e656087dfa53c0f8365a0c300da.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9682e656087dfa53c0f8365a0c300da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/567cd1355b86120b192d36b4710552a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/567cd1355b86120b192d36b4710552a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/327629df66c47aeba0cb92072cf94471.jpg\" _src=\"http://yanxuan.nosdn.127.net/327629df66c47aeba0cb92072cf94471.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31199ec47d032c282762d8d49087c5af.jpg\" _src=\"http://yanxuan.nosdn.127.net/31199ec47d032c282762d8d49087c5af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/169746e1e8293452b58c184db111d98b.jpg\" _src=\"http://yanxuan.nosdn.127.net/169746e1e8293452b58c184db111d98b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2a0cd32321cd198d67ea99fe5590120.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2a0cd32321cd198d67ea99fe5590120.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4657e1914acce0c476d756f72e40ef97.jpg\" _src=\"http://yanxuan.nosdn.127.net/4657e1914acce0c476d756f72e40ef97.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cb62e36a78ac61b587e6a9b5f9458a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cb62e36a78ac61b587e6a9b5f9458a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b482df93b0a173be4a7bf6c2dabd543.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b482df93b0a173be4a7bf6c2dabd543.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/533e784b613baea6c7d18ea81ce3b535.jpg\" _src=\"http://yanxuan.nosdn.127.net/533e784b613baea6c7d18ea81ce3b535.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15772709fdda505c1a3a6b0e6453cce8.jpg\" _src=\"http://yanxuan.nosdn.127.net/15772709fdda505c1a3a6b0e6453cce8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b8ffb1a51ec50d46707513e6d6cb420.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b8ffb1a51ec50d46707513e6d6cb420.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cf3463a41c5fac921cdb11c3b0c8990.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cf3463a41c5fac921cdb11c3b0c8990.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2565c92fa398dd47a1458be3e9009c9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/2565c92fa398dd47a1458be3e9009c9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a4960bb2a74c1e22d82626ba7e33d33d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a4960bb2a74c1e22d82626ba7e33d33d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c13f2fb5d0daac9ef6fab890c866dc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c13f2fb5d0daac9ef6fab890c866dc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/749704a3f974d419e8b59a32de540784.jpg\" _src=\"http://yanxuan.nosdn.127.net/749704a3f974d419e8b59a32de540784.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d1c4d8d91866700a5e8c1cd33ea75b15.jpg\" _src=\"http://yanxuan.nosdn.127.net/d1c4d8d91866700a5e8c1cd33ea75b15.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c55b8dc599470be31aa0218438a36528.jpg\" _src=\"http://yanxuan.nosdn.127.net/c55b8dc599470be31aa0218438a36528.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80c3a1e268905658a576eccd85a65f37.jpg\" _src=\"http://yanxuan.nosdn.127.net/80c3a1e268905658a576eccd85a65f37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c597a8dbecc1e3de31e9b8e5d420586.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c597a8dbecc1e3de31e9b8e5d420586.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/320ec6f1fcbb288e5676832dceff16aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/320ec6f1fcbb288e5676832dceff16aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8fc9119b2c7986bd575329d3a95abe9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8fc9119b2c7986bd575329d3a95abe9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/438a62f5bb789a6fa70b8ed5578cd7e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/438a62f5bb789a6fa70b8ed5578cd7e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1fe137a665f79a67359a9748de200ca6.jpg\" _src=\"http://yanxuan.nosdn.127.net/1fe137a665f79a67359a9748de200ca6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02ad092fac2cf5da935078f01afe3ff3.jpg\" _src=\"http://yanxuan.nosdn.127.net/02ad092fac2cf5da935078f01afe3ff3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d390285b49a6f4eb5ec9a460f77bce70.jpg\" _src=\"http://yanxuan.nosdn.127.net/d390285b49a6f4eb5ec9a460f77bce70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/469c7bc6e70c8d3db7639dc3d6949356.jpg\" _src=\"http://yanxuan.nosdn.127.net/469c7bc6e70c8d3db7639dc3d6949356.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/323b6604e88a5c748b4f7cd00ca84595.jpg\" _src=\"http://yanxuan.nosdn.127.net/323b6604e88a5c748b4f7cd00ca84595.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4151a8c4cae3b9998c95ae0bd9528e93.jpg\" _src=\"http://yanxuan.nosdn.127.net/4151a8c4cae3b9998c95ae0bd9528e93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c968e429b7a1f21ffa6281c76fd77c32.jpg\" _src=\"http://yanxuan.nosdn.127.net/c968e429b7a1f21ffa6281c76fd77c32.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 12,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 1,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/1f4758a9d68c5ebfafd3fc8b960707a6.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/aa49dfe878becf768eddc4c1636643a6.png",
      "retail_price": 46,
      "sell_volume": 7580,
      "primary_product_id": 1135146,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1134032,
      "category_id": 1008002,
      "goods_sn": "1134032",
      "name": "趣味粉彩系列记忆棉坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "慢回弹海绵的呵护，萌趣添彩。",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/ecbd6f05e8fc71571d889324e2f0dcad.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecbd6f05e8fc71571d889324e2f0dcad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bcdbec6d1b2ff457a0e7513df91563f0.jpg\" _src=\"http://yanxuan.nosdn.127.net/bcdbec6d1b2ff457a0e7513df91563f0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dcb21741c5c773e06cf4502925c81944.jpg\" _src=\"http://yanxuan.nosdn.127.net/dcb21741c5c773e06cf4502925c81944.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/86ffdbf55ae77e3c21a07a70445deda8.jpg\" _src=\"http://yanxuan.nosdn.127.net/86ffdbf55ae77e3c21a07a70445deda8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/598afa2e998b37d2c7513e7ab3a3ab73.jpg\" _src=\"http://yanxuan.nosdn.127.net/598afa2e998b37d2c7513e7ab3a3ab73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91dc47775ce962a1c2a7ac5e620f058c.jpg\" _src=\"http://yanxuan.nosdn.127.net/91dc47775ce962a1c2a7ac5e620f058c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/394b2bd47066e301a2144ab56b3b3350.jpg\" _src=\"http://yanxuan.nosdn.127.net/394b2bd47066e301a2144ab56b3b3350.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80dd29542f2ecd571db647486cda4e9f.jpg\" _src=\"http://yanxuan.nosdn.127.net/80dd29542f2ecd571db647486cda4e9f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a5edf27fe34192ed741ee8b011e8bcc.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a5edf27fe34192ed741ee8b011e8bcc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d2ee6fd1f0893f6c033b27f7353d1622.jpg\" _src=\"http://yanxuan.nosdn.127.net/d2ee6fd1f0893f6c033b27f7353d1622.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e11dd4cdab417eba665e0ad4ebc9243e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e11dd4cdab417eba665e0ad4ebc9243e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/feb11e4b1fb22d07533f11b59d6e602f.jpg\" _src=\"http://yanxuan.nosdn.127.net/feb11e4b1fb22d07533f11b59d6e602f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5094e4cf95940490ffccfad5db698301.jpg\" _src=\"http://yanxuan.nosdn.127.net/5094e4cf95940490ffccfad5db698301.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b0f9af05048828816c9a774124509dd0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b0f9af05048828816c9a774124509dd0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82020ae739c4ba0957db83b22c102673.jpg\" _src=\"http://yanxuan.nosdn.127.net/82020ae739c4ba0957db83b22c102673.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09789518f58c163313d5d4b190888500.jpg\" _src=\"http://yanxuan.nosdn.127.net/09789518f58c163313d5d4b190888500.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d155f2f1d12b54e5dfc83e3d3496dc2.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d155f2f1d12b54e5dfc83e3d3496dc2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44d1b96c7810379c6b48d58e637cba55.jpg\" _src=\"http://yanxuan.nosdn.127.net/44d1b96c7810379c6b48d58e637cba55.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c2075c17cf5c447d27c89f23d2d63462.jpg\" _src=\"http://yanxuan.nosdn.127.net/c2075c17cf5c447d27c89f23d2d63462.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3985bdbdb5899bee08137ab2300f3810.jpg\" _src=\"http://yanxuan.nosdn.127.net/3985bdbdb5899bee08137ab2300f3810.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fe8a47c8056ed17d6e08ac715d3aee93.jpg\" _src=\"http://yanxuan.nosdn.127.net/fe8a47c8056ed17d6e08ac715d3aee93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31f98b129c846c333bb95db48c434271.jpg\" _src=\"http://yanxuan.nosdn.127.net/31f98b129c846c333bb95db48c434271.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/857e3041c75f5ffb2eeb394ca9e1211d.jpg\" _src=\"http://yanxuan.nosdn.127.net/857e3041c75f5ffb2eeb394ca9e1211d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b04c0a98d696e3ba0a37857bcca5ca4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b04c0a98d696e3ba0a37857bcca5ca4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33a9842b9e01b0629d56a4ae725611a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/33a9842b9e01b0629d56a4ae725611a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/296263f5dc5e365662203331a940d058.jpg\" _src=\"http://yanxuan.nosdn.127.net/296263f5dc5e365662203331a940d058.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25e32af7a35f9c3b1105d5e1dc163e8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/25e32af7a35f9c3b1105d5e1dc163e8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6efac795f3b6207cf090846887461d65.jpg\" _src=\"http://yanxuan.nosdn.127.net/6efac795f3b6207cf090846887461d65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9b1e2e1c90d1481c83460ff71eaa47e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9b1e2e1c90d1481c83460ff71eaa47e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ab77215a79e8d9cc93304ec139af08e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ab77215a79e8d9cc93304ec139af08e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5eaab9336750bddb5a88fddfae7d2fbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/5eaab9336750bddb5a88fddfae7d2fbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7046719cdf72538e69b0313587c8565.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7046719cdf72538e69b0313587c8565.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/748836f2589106b87efec1c6be06f93d.jpg\" _src=\"http://yanxuan.nosdn.127.net/748836f2589106b87efec1c6be06f93d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40da8c4bed171c0fbfa9f2089a2309d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/40da8c4bed171c0fbfa9f2089a2309d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/468ed6ff0bbee10ba15467bb7b75c202.jpg\" _src=\"http://yanxuan.nosdn.127.net/468ed6ff0bbee10ba15467bb7b75c202.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2e1f9262f85b3301a6c9780acfcbb75.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2e1f9262f85b3301a6c9780acfcbb75.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ef0c70c73bff6274be4c562e88a7d6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ef0c70c73bff6274be4c562e88a7d6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/720c18b1bd787c125d59aa8f8f4c8e61.jpg\" _src=\"http://yanxuan.nosdn.127.net/720c18b1bd787c125d59aa8f8f4c8e61.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc80af1a2b58ac83a5d65cb3fa02f3db.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc80af1a2b58ac83a5d65cb3fa02f3db.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/98d647cacddc7bdd7eae86050eb9f3d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/98d647cacddc7bdd7eae86050eb9f3d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a091331dc2412de558446a42831b0358.jpg\" _src=\"http://yanxuan.nosdn.127.net/a091331dc2412de558446a42831b0358.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd6126e6eb2a4e493104f75ecbeb6e32.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd6126e6eb2a4e493104f75ecbeb6e32.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d15ad6abec2f8c499c0d9d036a8b524.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d15ad6abec2f8c499c0d9d036a8b524.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69a56acc851dd042a52f18c78ac8ee33.jpg\" _src=\"http://yanxuan.nosdn.127.net/69a56acc851dd042a52f18c78ac8ee33.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8bde0e10b1e089088ca38fd77fbf994.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8bde0e10b1e089088ca38fd77fbf994.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd9ffb9b37957549689ece880fc78b2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd9ffb9b37957549689ece880fc78b2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09ad556caef32a5c951dc7fbad1f8de3.jpg\" _src=\"http://yanxuan.nosdn.127.net/09ad556caef32a5c951dc7fbad1f8de3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a919f989730d977f8b1745b5dc0e6a8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a919f989730d977f8b1745b5dc0e6a8d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 13,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 1,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/5357e0476acbc71131df5a3fb3ea13d9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/8b30eeb17c831eba08b97bdcb4c46a8e.png",
      "retail_price": 49,
      "sell_volume": 2869,
      "primary_product_id": 1135151,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135051,
      "category_id": 1008002,
      "goods_sn": "1135051",
      "name": "日式素雅纯色流星纹窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "日式素雅设计 流星纹简约肌理",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/70d4eceeb3f066bd4ea015fca75f424c.jpg\" _src=\"http://yanxuan.nosdn.127.net/70d4eceeb3f066bd4ea015fca75f424c.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebc7b596ef941847afe073a173bcfa59.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebc7b596ef941847afe073a173bcfa59.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c14d1ecbff1c587aefd16d65b47cae51.jpg\" _src=\"http://yanxuan.nosdn.127.net/c14d1ecbff1c587aefd16d65b47cae51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d269aeec1f4410c68b2f2c3f77f7985.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d269aeec1f4410c68b2f2c3f77f7985.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ae8263c89b5fbc0de5df0c21d67d3d2.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ae8263c89b5fbc0de5df0c21d67d3d2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/915f66ecc21197b4d99b5c3df5cbffab.jpg\" _src=\"http://yanxuan.nosdn.127.net/915f66ecc21197b4d99b5c3df5cbffab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4781c28a5295b239075883ccaa0a9c74.jpg\" _src=\"http://yanxuan.nosdn.127.net/4781c28a5295b239075883ccaa0a9c74.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91a4983796259d464e1f3795da189a17.jpg\" _src=\"http://yanxuan.nosdn.127.net/91a4983796259d464e1f3795da189a17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3950395fcc7e7fdc388a2ccf2b6ac0e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/3950395fcc7e7fdc388a2ccf2b6ac0e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9112abffdf6edd3b0ab8f9fb364d84f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/9112abffdf6edd3b0ab8f9fb364d84f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/96dcd6ccfec216bf2ce45393ca0aead1.jpg\" _src=\"http://yanxuan.nosdn.127.net/96dcd6ccfec216bf2ce45393ca0aead1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6dffe4e2cce9fb45abe1182bcb1939e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/6dffe4e2cce9fb45abe1182bcb1939e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d358645610f642ef7fd262c0101790e0.jpg\" _src=\"http://yanxuan.nosdn.127.net/d358645610f642ef7fd262c0101790e0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb51ccf74568565ba366f0eabf54ccbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb51ccf74568565ba366f0eabf54ccbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7517d9dc2d70be25722a009083ed82df.jpg\" _src=\"http://yanxuan.nosdn.127.net/7517d9dc2d70be25722a009083ed82df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11deb1b2b5efa58291c8a62355df6017.jpg\" _src=\"http://yanxuan.nosdn.127.net/11deb1b2b5efa58291c8a62355df6017.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/172053c17a9a97a8108f8fd170a6b07f.jpg\" _src=\"http://yanxuan.nosdn.127.net/172053c17a9a97a8108f8fd170a6b07f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a1c0ac59021d408dcd9845c8702522a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a1c0ac59021d408dcd9845c8702522a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/781d08f49d1870ac9cf8b93dacfbf711.jpg\" _src=\"http://yanxuan.nosdn.127.net/781d08f49d1870ac9cf8b93dacfbf711.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b764a61f92c6db3440f6b4aed6a7625.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b764a61f92c6db3440f6b4aed6a7625.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31ec911d03541ace9eddfbf3fcdf0414.jpg\" _src=\"http://yanxuan.nosdn.127.net/31ec911d03541ace9eddfbf3fcdf0414.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9d602c94b739bb01da939d75a9187a16.jpg\" _src=\"http://yanxuan.nosdn.127.net/9d602c94b739bb01da939d75a9187a16.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc557a3e4478f089973519699a01c01c.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc557a3e4478f089973519699a01c01c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1efdae30fe5189bb998509d446ff271.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1efdae30fe5189bb998509d446ff271.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/12116c10da83b5835a36315711640765.jpg\" _src=\"http://yanxuan.nosdn.127.net/12116c10da83b5835a36315711640765.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9491370cd9c5486fd9aa22ef9fdbd6fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/9491370cd9c5486fd9aa22ef9fdbd6fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37ca15cf48249bc390fcc05077741b98.jpg\" _src=\"http://yanxuan.nosdn.127.net/37ca15cf48249bc390fcc05077741b98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99fec7d83ae7e82a4426d3859875d8c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/99fec7d83ae7e82a4426d3859875d8c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9912fa7c176dc1b64c060992eb40b60.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9912fa7c176dc1b64c060992eb40b60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a04c0b364a1fa322ca6a71f35708e3ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/a04c0b364a1fa322ca6a71f35708e3ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8604f596b1d0703547d40608dfe16f2a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8604f596b1d0703547d40608dfe16f2a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b86422ab0ffe13da8f627245ec4dc98.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b86422ab0ffe13da8f627245ec4dc98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b2d3c68d23acb03a3c542cccb301bfb.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b2d3c68d23acb03a3c542cccb301bfb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d563205fb46fc71c3c37448673f5e714.jpg\" _src=\"http://yanxuan.nosdn.127.net/d563205fb46fc71c3c37448673f5e714.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18efa2d731c643a56a2976b4c793eec2.jpg\" _src=\"http://yanxuan.nosdn.127.net/18efa2d731c643a56a2976b4c793eec2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b644146188b5ceba4b86ec82352f660.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b644146188b5ceba4b86ec82352f660.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9c51c9c2c94f28102cb516656c7c761.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9c51c9c2c94f28102cb516656c7c761.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/769660ddc2ad27a1e62543460ff2bc41.jpg\" _src=\"http://yanxuan.nosdn.127.net/769660ddc2ad27a1e62543460ff2bc41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c95e64b4454063ba74c8cb17a95d60cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/c95e64b4454063ba74c8cb17a95d60cf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9a79d20d29a65bd010cf084c7b783d96.jpg\" _src=\"http://yanxuan.nosdn.127.net/9a79d20d29a65bd010cf084c7b783d96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18a89642689470308392fa485a633709.jpg\" _src=\"http://yanxuan.nosdn.127.net/18a89642689470308392fa485a633709.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/706c31eaec80f9417fbcdd40c16a7f63.jpg\" _src=\"http://yanxuan.nosdn.127.net/706c31eaec80f9417fbcdd40c16a7f63.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bec2e276673ab2787f03b8bd444044af.jpg\" _src=\"http://yanxuan.nosdn.127.net/bec2e276673ab2787f03b8bd444044af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3afb40257bc5fac38369dd465fe7732c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3afb40257bc5fac38369dd465fe7732c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cfe30745d27efdc8080944bd8d8c927.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cfe30745d27efdc8080944bd8d8c927.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e3aabaab6a42e859c2362998f235a564.jpg\" _src=\"http://yanxuan.nosdn.127.net/e3aabaab6a42e859c2362998f235a564.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6946e6dfe5a3026c67672c69061a06ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/6946e6dfe5a3026c67672c69061a06ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/778f89a8b141f03b6fcb206692b37d7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/778f89a8b141f03b6fcb206692b37d7f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b991c295b7bc2f6a6e04f7e79cede25.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b991c295b7bc2f6a6e04f7e79cede25.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e3f9724481dda6c024854750a3aeaa2.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e3f9724481dda6c024854750a3aeaa2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48bc347fe73c771d19787229da647421.jpg\" _src=\"http://yanxuan.nosdn.127.net/48bc347fe73c771d19787229da647421.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7a2a0bfe4036e4c3add5ba33313da069.jpg\" _src=\"http://yanxuan.nosdn.127.net/7a2a0bfe4036e4c3add5ba33313da069.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ec518bd9a7f9914841cc92e3e52fa45.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ec518bd9a7f9914841cc92e3e52fa45.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3054be42bc630607c3a46a9fe2ce6ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3054be42bc630607c3a46a9fe2ce6ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b368f5bd63b6b59b2064af102a1fa8e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b368f5bd63b6b59b2064af102a1fa8e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dda7a836f7a7c54256b35253bbfba90f.jpg\" _src=\"http://yanxuan.nosdn.127.net/dda7a836f7a7c54256b35253bbfba90f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91216189bef9aa48018bbf8e654443ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/91216189bef9aa48018bbf8e654443ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10b8c1cace53090fe30a9834365ee37e.jpg\" _src=\"http://yanxuan.nosdn.127.net/10b8c1cace53090fe30a9834365ee37e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbf5782db6be5a01de6d0cf1c64eea30.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbf5782db6be5a01de6d0cf1c64eea30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c49df712817bfe30ec83a26af1b8b1de.jpg\" _src=\"http://yanxuan.nosdn.127.net/c49df712817bfe30ec83a26af1b8b1de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/510c05dc331823949d1567c552562a9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/510c05dc331823949d1567c552562a9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c673ce9d4d825503402f1c352b8e82ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/c673ce9d4d825503402f1c352b8e82ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/378135cf12f5c044871b59c060cacbb9.jpg\" _src=\"http://yanxuan.nosdn.127.net/378135cf12f5c044871b59c060cacbb9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd58aebd08f03474c7ed159c005a986c.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd58aebd08f03474c7ed159c005a986c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5a99049b512e9a388ffb1520827b2739.jpg\" _src=\"http://yanxuan.nosdn.127.net/5a99049b512e9a388ffb1520827b2739.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa65626e5df752d70ae4662d1b15dc8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa65626e5df752d70ae4662d1b15dc8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84d1dcf5083fd69abf4451a660f31d59.jpg\" _src=\"http://yanxuan.nosdn.127.net/84d1dcf5083fd69abf4451a660f31d59.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f781abaecbfb60889be6f46f83f4069.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f781abaecbfb60889be6f46f83f4069.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/26a745d26c76a4577feaf58b27ff557b.jpg\" _src=\"http://yanxuan.nosdn.127.net/26a745d26c76a4577feaf58b27ff557b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/887eb48649e1db53f3047340404209f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/887eb48649e1db53f3047340404209f6.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 35,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/95dbdb2e63eeed44c4a40ea586ad4196.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/9126151f028a8804026d530836b481cb.png",
      "retail_price": 299,
      "sell_volume": 1816,
      "primary_product_id": 1136377,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135052,
      "category_id": 1008002,
      "goods_sn": "1135052",
      "name": "日式简约素色窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "日式极简美学 舒适棉麻质感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/2edc19a016d64d3b29aa71b0bf6cc928.jpg\" _src=\"http://yanxuan.nosdn.127.net/2edc19a016d64d3b29aa71b0bf6cc928.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bdc1fc55629dbfccbdfaa6b17ebfacc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bdc1fc55629dbfccbdfaa6b17ebfacc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4ef1e93a0d3f71d7862441ffd922e522.jpg\" _src=\"http://yanxuan.nosdn.127.net/4ef1e93a0d3f71d7862441ffd922e522.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85a1e175e39a6576dffb2f0ca28597f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/85a1e175e39a6576dffb2f0ca28597f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/486aedd7ce019d1c465bf8bbf77314bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/486aedd7ce019d1c465bf8bbf77314bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9f8f7045f07d1bb742f67120009afd0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9f8f7045f07d1bb742f67120009afd0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c813c0a23951007b020b9b03d0f31cb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c813c0a23951007b020b9b03d0f31cb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9a87cebbc5b127abf6a6e5129d4ed20c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9a87cebbc5b127abf6a6e5129d4ed20c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38e85411821a681c2dd5a5b9bd3cab92.jpg\" _src=\"http://yanxuan.nosdn.127.net/38e85411821a681c2dd5a5b9bd3cab92.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3907fa867c71f4090699898d53b937d.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3907fa867c71f4090699898d53b937d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c284309b66cc8d073f528c7ebf78c5fb.jpg\" _src=\"http://yanxuan.nosdn.127.net/c284309b66cc8d073f528c7ebf78c5fb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ecb27fc699a97883f7d14c7e606daa3.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ecb27fc699a97883f7d14c7e606daa3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eaf351d46c216f2f3a3588b3985d18c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/eaf351d46c216f2f3a3588b3985d18c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/785ab1ac578124415bbd718813413333.jpg\" _src=\"http://yanxuan.nosdn.127.net/785ab1ac578124415bbd718813413333.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8605647112b62e72f78ee27d29eede3d.jpg\" _src=\"http://yanxuan.nosdn.127.net/8605647112b62e72f78ee27d29eede3d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3952310896b95dcdc3adb986e5487a86.jpg\" _src=\"http://yanxuan.nosdn.127.net/3952310896b95dcdc3adb986e5487a86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/030f115457262723b3d821987e38b111.jpg\" _src=\"http://yanxuan.nosdn.127.net/030f115457262723b3d821987e38b111.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf4254e1d4962d6e9f5e4734785f57ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf4254e1d4962d6e9f5e4734785f57ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce29d7cdc0e56477a623d03856646448.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce29d7cdc0e56477a623d03856646448.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/515086ca9168f8008291e98a01f4e4c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/515086ca9168f8008291e98a01f4e4c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9bb9d186d4a364ed0c91606d561a7f5.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9bb9d186d4a364ed0c91606d561a7f5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63204b444e0d06a7fafb6c5e35153eaa.jpg\" _src=\"http://yanxuan.nosdn.127.net/63204b444e0d06a7fafb6c5e35153eaa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d13212d5d43f766d3f5c37ccb4e5714.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d13212d5d43f766d3f5c37ccb4e5714.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19d5b4dbb590d90c3e40525a3ef35019.jpg\" _src=\"http://yanxuan.nosdn.127.net/19d5b4dbb590d90c3e40525a3ef35019.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0a1fcdbac2d1bf232e95389e20ed07c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0a1fcdbac2d1bf232e95389e20ed07c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d230fbda487cf445cd57f4296b7a487.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d230fbda487cf445cd57f4296b7a487.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5819e9bbdeda97281990f61c531fdbbb.jpg\" _src=\"http://yanxuan.nosdn.127.net/5819e9bbdeda97281990f61c531fdbbb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/802799f78d7069fc4dc44ff339729dc9.jpg\" _src=\"http://yanxuan.nosdn.127.net/802799f78d7069fc4dc44ff339729dc9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de5108481df4cbc2e064a1fcc477475f.jpg\" _src=\"http://yanxuan.nosdn.127.net/de5108481df4cbc2e064a1fcc477475f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a94262fecc2427d613ad7cbdd0a59f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a94262fecc2427d613ad7cbdd0a59f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b18c9c41d0520d1e0f1b58a7ae13e5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b18c9c41d0520d1e0f1b58a7ae13e5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/564d7115798352b765da2633949a1818.jpg\" _src=\"http://yanxuan.nosdn.127.net/564d7115798352b765da2633949a1818.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f84553b8cfa29fb222b17bc89140fa9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f84553b8cfa29fb222b17bc89140fa9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b01288738e632c5afda98184bb62095.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b01288738e632c5afda98184bb62095.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23088788bbfd7bf4b60ee06e9722ed74.jpg\" _src=\"http://yanxuan.nosdn.127.net/23088788bbfd7bf4b60ee06e9722ed74.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b2a400e968802cd64d31bdc038b3e2a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b2a400e968802cd64d31bdc038b3e2a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b0e31fe278c7704fed496ea82c679044.jpg\" _src=\"http://yanxuan.nosdn.127.net/b0e31fe278c7704fed496ea82c679044.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2054d55fc3bdaa380ce28c1fa9b4b00d.jpg\" _src=\"http://yanxuan.nosdn.127.net/2054d55fc3bdaa380ce28c1fa9b4b00d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d03bae43ba821cd933d0e652e9d3bb7.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d03bae43ba821cd933d0e652e9d3bb7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc1c458d99de149af69d8ac7582b72dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc1c458d99de149af69d8ac7582b72dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b92c88836f39dfc194d7e56cfdfcaf5c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b92c88836f39dfc194d7e56cfdfcaf5c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1446a01f9725a03ca79ab3e57fdc181a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1446a01f9725a03ca79ab3e57fdc181a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63fb7826d9f2d34f22317110d60a5b9d.jpg\" _src=\"http://yanxuan.nosdn.127.net/63fb7826d9f2d34f22317110d60a5b9d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91b1dced907315eb0e771a504d29e6d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/91b1dced907315eb0e771a504d29e6d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/985d212a97d26d4ff1029ee4efdbc4f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/985d212a97d26d4ff1029ee4efdbc4f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8978ab0059b90f8b018b1de05fa4e8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8978ab0059b90f8b018b1de05fa4e8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25f62074f6e7e3e2b95a71e32aa43311.jpg\" _src=\"http://yanxuan.nosdn.127.net/25f62074f6e7e3e2b95a71e32aa43311.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e8fa97196d22fb3bbc4cd871267cc79.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e8fa97196d22fb3bbc4cd871267cc79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c3478950cc4f473849ed3ab3de21bd4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c3478950cc4f473849ed3ab3de21bd4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/838a150e46e5720a78f61ac48d380891.jpg\" _src=\"http://yanxuan.nosdn.127.net/838a150e46e5720a78f61ac48d380891.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2abd7db65b092e91ce87c09bf4c4c17f.jpg\" _src=\"http://yanxuan.nosdn.127.net/2abd7db65b092e91ce87c09bf4c4c17f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e603a799d802123ceaf5dbf3de02b051.jpg\" _src=\"http://yanxuan.nosdn.127.net/e603a799d802123ceaf5dbf3de02b051.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8460ba6d6347be878f035b7457ec9057.jpg\" _src=\"http://yanxuan.nosdn.127.net/8460ba6d6347be878f035b7457ec9057.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b02f932cfd15a19a2f1cebfab19b2cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b02f932cfd15a19a2f1cebfab19b2cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41fe9fb3c58a41023a74ef1740573fec.jpg\" _src=\"http://yanxuan.nosdn.127.net/41fe9fb3c58a41023a74ef1740573fec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19cc0338b0efefe7f0140efde638c705.jpg\" _src=\"http://yanxuan.nosdn.127.net/19cc0338b0efefe7f0140efde638c705.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e670a47f65733d99c4884f90b49d8e6.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e670a47f65733d99c4884f90b49d8e6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4859ec0aeecc39ed751f2a07daecad10.jpg\" _src=\"http://yanxuan.nosdn.127.net/4859ec0aeecc39ed751f2a07daecad10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b7b2a56a1ea98119e89ae93b71e68c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b7b2a56a1ea98119e89ae93b71e68c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6e9767a0f40cbaf19307bd0c1ef97df9.jpg\" _src=\"http://yanxuan.nosdn.127.net/6e9767a0f40cbaf19307bd0c1ef97df9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ca04a1436a6598858fc74db1f571529.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ca04a1436a6598858fc74db1f571529.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/738fc25303e4bb32d1efe45641f1b120.jpg\" _src=\"http://yanxuan.nosdn.127.net/738fc25303e4bb32d1efe45641f1b120.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c5de7c6679cfe0361ac9d164276739ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/c5de7c6679cfe0361ac9d164276739ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e1edc1ea0bcc4cd92134ce8cc775577.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e1edc1ea0bcc4cd92134ce8cc775577.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e1eaacf6e5dc52fecb3e9c889db2ee32.jpg\" _src=\"http://yanxuan.nosdn.127.net/e1eaacf6e5dc52fecb3e9c889db2ee32.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/78cea538e5017c2782a96e215f42d6f3.jpg\" _src=\"http://yanxuan.nosdn.127.net/78cea538e5017c2782a96e215f42d6f3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f268a66c2e2476c075dd87416790b761.jpg\" _src=\"http://yanxuan.nosdn.127.net/f268a66c2e2476c075dd87416790b761.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9f6900f77c23e57a0a2633554ce0c8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9f6900f77c23e57a0a2633554ce0c8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9db7f3c92e24143e8ece310935785e41.jpg\" _src=\"http://yanxuan.nosdn.127.net/9db7f3c92e24143e8ece310935785e41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/923a8a571519b89b1a03e898871ef586.jpg\" _src=\"http://yanxuan.nosdn.127.net/923a8a571519b89b1a03e898871ef586.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 34,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/38129b4cdabcdf5610160d3a15ef259b.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/63f5da1f5363af43aa91864bf66af48e.png",
      "retail_price": 259,
      "sell_volume": 2776,
      "primary_product_id": 1136402,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135053,
      "category_id": 1008002,
      "goods_sn": "1135053",
      "name": "法式复古山形纹提花窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "轻奢复古，立体提花",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/e21a28b9c5e5203d217f54b0dec35735.jpg\" _src=\"http://yanxuan.nosdn.127.net/e21a28b9c5e5203d217f54b0dec35735.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/49e4de111eb6cf9ba70ee5ed8c85a416.jpg\" _src=\"http://yanxuan.nosdn.127.net/49e4de111eb6cf9ba70ee5ed8c85a416.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba9e72450a61c5259c0e025b155d58cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba9e72450a61c5259c0e025b155d58cf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41dc601d1494f0775e4763091a6671ca.jpg\" _src=\"http://yanxuan.nosdn.127.net/41dc601d1494f0775e4763091a6671ca.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d55bfd606020ef7de66bd70a1b93a12f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d55bfd606020ef7de66bd70a1b93a12f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bc7c6fa620e2635cced6ffbcfd4e6c49.jpg\" _src=\"http://yanxuan.nosdn.127.net/bc7c6fa620e2635cced6ffbcfd4e6c49.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a038525d854188e43cacd3ad2bf9a7a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/a038525d854188e43cacd3ad2bf9a7a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6224e8afea6653f1baaf9eceb70f4d1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/6224e8afea6653f1baaf9eceb70f4d1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/617f4b84e19adb6a5e81cf5c3a5574e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/617f4b84e19adb6a5e81cf5c3a5574e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5265f7746597699562be16e8cd367e78.jpg\" _src=\"http://yanxuan.nosdn.127.net/5265f7746597699562be16e8cd367e78.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7be914365886d471a418ca767e8b2432.jpg\" _src=\"http://yanxuan.nosdn.127.net/7be914365886d471a418ca767e8b2432.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2dce0091a62324d69685980ce463c8e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/2dce0091a62324d69685980ce463c8e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f190e680db954313c315ff788c2e677.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f190e680db954313c315ff788c2e677.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/349da9942e82dcc44629781ef2254c06.jpg\" _src=\"http://yanxuan.nosdn.127.net/349da9942e82dcc44629781ef2254c06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9829be8b12dda40cec3c844df9e521b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/9829be8b12dda40cec3c844df9e521b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/082cb3197ad814c2df6f6089fa00fa46.jpg\" _src=\"http://yanxuan.nosdn.127.net/082cb3197ad814c2df6f6089fa00fa46.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca9038261114bdc03cb44ebabacaa67e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca9038261114bdc03cb44ebabacaa67e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b4808db6982d4c6efb9967d3e0aad71.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b4808db6982d4c6efb9967d3e0aad71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b5f9b19c256980f8948b7eec4319f7e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b5f9b19c256980f8948b7eec4319f7e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fbe8e4222a5dbb5a34b774374377c60.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fbe8e4222a5dbb5a34b774374377c60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3981672ef8bba7d656e1f6a439b2049.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3981672ef8bba7d656e1f6a439b2049.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/389a17a26b55ebd8090514087ed8b573.jpg\" _src=\"http://yanxuan.nosdn.127.net/389a17a26b55ebd8090514087ed8b573.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/577e2ba58b6c716b1f1e02d95992f8cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/577e2ba58b6c716b1f1e02d95992f8cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/deb4940d64591b194395c14f2d5407dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/deb4940d64591b194395c14f2d5407dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c0cce63ad9658252ddb9152a0801c69.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c0cce63ad9658252ddb9152a0801c69.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/51f7db1d8a7288aaf9712f978dd0e808.jpg\" _src=\"http://yanxuan.nosdn.127.net/51f7db1d8a7288aaf9712f978dd0e808.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09c3bdf807406fe5fe345e875ac4a69d.jpg\" _src=\"http://yanxuan.nosdn.127.net/09c3bdf807406fe5fe345e875ac4a69d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/818d25244f2dfdade6b23a4a92f55a51.jpg\" _src=\"http://yanxuan.nosdn.127.net/818d25244f2dfdade6b23a4a92f55a51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/310d4c4888d21f9100d36d7b19b7b841.jpg\" _src=\"http://yanxuan.nosdn.127.net/310d4c4888d21f9100d36d7b19b7b841.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb8e667ad88260e90211a4f9b246f8e4.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb8e667ad88260e90211a4f9b246f8e4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2b75ffc95e4a5c69944b99b7d3f04837.jpg\" _src=\"http://yanxuan.nosdn.127.net/2b75ffc95e4a5c69944b99b7d3f04837.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfef40e5a0861fb9e958b0a6a70c8cf8.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfef40e5a0861fb9e958b0a6a70c8cf8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a506fed177d609e43be43c4eb4ed0c6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/a506fed177d609e43be43c4eb4ed0c6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a6c905743a3c03c679c7017701399e1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/a6c905743a3c03c679c7017701399e1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2e44ac8c851c24ff28ef3d28fca1e363.jpg\" _src=\"http://yanxuan.nosdn.127.net/2e44ac8c851c24ff28ef3d28fca1e363.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d121846341c4eec125668560ea59606.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d121846341c4eec125668560ea59606.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbf82173395352acae173a6acac219c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbf82173395352acae173a6acac219c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8e6aff62f8304cf4c9847f1e6844407.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8e6aff62f8304cf4c9847f1e6844407.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a604d607f42ad8a1c343d604cc4c147.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a604d607f42ad8a1c343d604cc4c147.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/775d13d9704afa2a46ae2d6616ff78ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/775d13d9704afa2a46ae2d6616ff78ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65617bbfc95b22a4a6fb6060781afc70.jpg\" _src=\"http://yanxuan.nosdn.127.net/65617bbfc95b22a4a6fb6060781afc70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79613c75ad103b7b0cc1933a62afeff7.jpg\" _src=\"http://yanxuan.nosdn.127.net/79613c75ad103b7b0cc1933a62afeff7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9754dd885b4f1ff698b440d8582fda5b.jpg\" _src=\"http://yanxuan.nosdn.127.net/9754dd885b4f1ff698b440d8582fda5b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/372bbb746116a10e5c82d2c136883472.jpg\" _src=\"http://yanxuan.nosdn.127.net/372bbb746116a10e5c82d2c136883472.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79466f6b09420a3c8e8e39ab2091c32e.jpg\" _src=\"http://yanxuan.nosdn.127.net/79466f6b09420a3c8e8e39ab2091c32e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/852fce888e2e4abd8e9256207ce8857c.jpg\" _src=\"http://yanxuan.nosdn.127.net/852fce888e2e4abd8e9256207ce8857c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f51d785e3ecbe7da3abfb03527900ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f51d785e3ecbe7da3abfb03527900ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdf18ac18c0bc4a9ca2834d14bc67e40.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdf18ac18c0bc4a9ca2834d14bc67e40.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/64a9503d1375d2ce3cf2d3aaa8f49d0a.jpg\" _src=\"http://yanxuan.nosdn.127.net/64a9503d1375d2ce3cf2d3aaa8f49d0a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc7ea083ed7bee671c2b34fdf0a29837.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc7ea083ed7bee671c2b34fdf0a29837.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e58086a3385b0dcb915a35607e83a676.jpg\" _src=\"http://yanxuan.nosdn.127.net/e58086a3385b0dcb915a35607e83a676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/239a602da7415684a44d5421ebb71e77.jpg\" _src=\"http://yanxuan.nosdn.127.net/239a602da7415684a44d5421ebb71e77.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c8ecca60b20a9f891c18adc051b7fbc.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c8ecca60b20a9f891c18adc051b7fbc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf21f6ceb63279ceccbc35c882c9030c.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf21f6ceb63279ceccbc35c882c9030c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7865fb8acee04157b94b85e62b6f2d14.jpg\" _src=\"http://yanxuan.nosdn.127.net/7865fb8acee04157b94b85e62b6f2d14.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3c1797e21327d8bff828ac761305867.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3c1797e21327d8bff828ac761305867.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3263b186f04be03faa803dacf2bddcd.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3263b186f04be03faa803dacf2bddcd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0a0bfa53b619a61d143314d60e13341.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0a0bfa53b619a61d143314d60e13341.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e3ddada3bf508947a5715df6792c980.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e3ddada3bf508947a5715df6792c980.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ee6d2c940700caeec4997ff6deeca4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ee6d2c940700caeec4997ff6deeca4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3902aa67f3485894c892eef84be25952.jpg\" _src=\"http://yanxuan.nosdn.127.net/3902aa67f3485894c892eef84be25952.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9779fa93d513d2747aada4f83423df22.jpg\" _src=\"http://yanxuan.nosdn.127.net/9779fa93d513d2747aada4f83423df22.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4da023d34922ad0fc42ce5e4ac0e3431.jpg\" _src=\"http://yanxuan.nosdn.127.net/4da023d34922ad0fc42ce5e4ac0e3431.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5da0d3862a5e5f72b020a396fcc77423.jpg\" _src=\"http://yanxuan.nosdn.127.net/5da0d3862a5e5f72b020a396fcc77423.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f99a92c12c7057fd5dad948bb80cff98.jpg\" _src=\"http://yanxuan.nosdn.127.net/f99a92c12c7057fd5dad948bb80cff98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9453c191e802aeb86241cee2e2dd70a5.jpg\" _src=\"http://yanxuan.nosdn.127.net/9453c191e802aeb86241cee2e2dd70a5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/225ab93dd58a18f5878c57841c18b8ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/225ab93dd58a18f5878c57841c18b8ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/57994f32bd6423bed216a80c8456eafc.jpg\" _src=\"http://yanxuan.nosdn.127.net/57994f32bd6423bed216a80c8456eafc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9803612c814317b259e6c244fb3e191.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9803612c814317b259e6c244fb3e191.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 38,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/3235e120465f2755b6a412668d0be967.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/1f9e34b1aadd14ea0c9c299c530d86ba.png",
      "retail_price": 429,
      "sell_volume": 5280,
      "primary_product_id": 1136424,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135054,
      "category_id": 1008002,
      "goods_sn": "1135054",
      "name": "美式田园风蜻蜓提花窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "美式蜻蜓提花 甜美田园色彩",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/8b13ceefdeffbfd2b2326b9429ab7896.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b13ceefdeffbfd2b2326b9429ab7896.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8fa854947a7df61a4e063b8e2e14fd3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8fa854947a7df61a4e063b8e2e14fd3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d9681a7dd16355294e37057fa3b6c64.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d9681a7dd16355294e37057fa3b6c64.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/292b9704967295fcbf09ee7a98b40425.jpg\" _src=\"http://yanxuan.nosdn.127.net/292b9704967295fcbf09ee7a98b40425.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2ba9a3fb827a7c135670655ff4060553.jpg\" _src=\"http://yanxuan.nosdn.127.net/2ba9a3fb827a7c135670655ff4060553.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0b12070b3da9c44102a91b34d4a289d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0b12070b3da9c44102a91b34d4a289d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27a0e45f6cb8db4e541cc09dc3f56661.jpg\" _src=\"http://yanxuan.nosdn.127.net/27a0e45f6cb8db4e541cc09dc3f56661.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/78c39affb31ea084aec9092a528e1000.jpg\" _src=\"http://yanxuan.nosdn.127.net/78c39affb31ea084aec9092a528e1000.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1dbf236c3d1f41e23bb703be8e09d62.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1dbf236c3d1f41e23bb703be8e09d62.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8a10b18efc6670c4b5c6abfe25a5d791.jpg\" _src=\"http://yanxuan.nosdn.127.net/8a10b18efc6670c4b5c6abfe25a5d791.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31f310bfa2a088a865ba86d603c889e3.jpg\" _src=\"http://yanxuan.nosdn.127.net/31f310bfa2a088a865ba86d603c889e3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6e1112e5c699aadb80edf862b013241.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6e1112e5c699aadb80edf862b013241.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70e35f2b7536dcf59061fb15e6fbd7f0.jpg\" _src=\"http://yanxuan.nosdn.127.net/70e35f2b7536dcf59061fb15e6fbd7f0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fab87a9493b50f6372eab5d02ab58ddc.jpg\" _src=\"http://yanxuan.nosdn.127.net/fab87a9493b50f6372eab5d02ab58ddc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6431ef7fa249e9e0412eceac99d77acb.jpg\" _src=\"http://yanxuan.nosdn.127.net/6431ef7fa249e9e0412eceac99d77acb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6a3e40285e7e1ba47fff926acd7fb02.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6a3e40285e7e1ba47fff926acd7fb02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d714470698ed5f14cf21ca34f3012bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d714470698ed5f14cf21ca34f3012bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9bc9c660db31968471b598a293b3c44b.jpg\" _src=\"http://yanxuan.nosdn.127.net/9bc9c660db31968471b598a293b3c44b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1bb7a825a3148cb187e8ec2d39b60f21.jpg\" _src=\"http://yanxuan.nosdn.127.net/1bb7a825a3148cb187e8ec2d39b60f21.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9097e4911884ae79e055d85ba0cc07b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/9097e4911884ae79e055d85ba0cc07b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/49195539f093b5974392cef9f3b2c5c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/49195539f093b5974392cef9f3b2c5c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71dc1d77d97e2495dea6edd66b62e906.jpg\" _src=\"http://yanxuan.nosdn.127.net/71dc1d77d97e2495dea6edd66b62e906.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbb3af413fa229c94682dea4e959edbe.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbb3af413fa229c94682dea4e959edbe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3a2b3bcda99806ff31844d44537f62e.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3a2b3bcda99806ff31844d44537f62e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e09dbf79c01d9ec02234be2063fade0.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e09dbf79c01d9ec02234be2063fade0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2838ac897fbc4339701789d3e05b176e.jpg\" _src=\"http://yanxuan.nosdn.127.net/2838ac897fbc4339701789d3e05b176e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/efe9c94a8e77081d69e8f30dfb501bc6.jpg\" _src=\"http://yanxuan.nosdn.127.net/efe9c94a8e77081d69e8f30dfb501bc6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2d8913b07b679efe4349802d9b0a6887.jpg\" _src=\"http://yanxuan.nosdn.127.net/2d8913b07b679efe4349802d9b0a6887.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aad09d61a369e2828a64996e6f594331.jpg\" _src=\"http://yanxuan.nosdn.127.net/aad09d61a369e2828a64996e6f594331.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09a0cc37d89dc0b604a69806ea1a1ec7.jpg\" _src=\"http://yanxuan.nosdn.127.net/09a0cc37d89dc0b604a69806ea1a1ec7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/680758fc7cf2315433ff5815b42a1620.jpg\" _src=\"http://yanxuan.nosdn.127.net/680758fc7cf2315433ff5815b42a1620.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6a83a5e81614a57ca3c55518130dc6e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/6a83a5e81614a57ca3c55518130dc6e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09474a7d70cb78b5baadd27906b09a48.jpg\" _src=\"http://yanxuan.nosdn.127.net/09474a7d70cb78b5baadd27906b09a48.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85ffaf2d542e988adce23e576f539a11.jpg\" _src=\"http://yanxuan.nosdn.127.net/85ffaf2d542e988adce23e576f539a11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d56fded6471b21499e524b041fd7f409.jpg\" _src=\"http://yanxuan.nosdn.127.net/d56fded6471b21499e524b041fd7f409.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/01d319f088e87d2c3c223467de321352.jpg\" _src=\"http://yanxuan.nosdn.127.net/01d319f088e87d2c3c223467de321352.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2800c131d7320919b6b02adae7e5bd9.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2800c131d7320919b6b02adae7e5bd9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8172ab2121042e5703183b43fd195509.jpg\" _src=\"http://yanxuan.nosdn.127.net/8172ab2121042e5703183b43fd195509.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40dbb2286998622b9902fc704b583040.jpg\" _src=\"http://yanxuan.nosdn.127.net/40dbb2286998622b9902fc704b583040.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/68e4e99f2a0a400bfade8cd2befd0e69.jpg\" _src=\"http://yanxuan.nosdn.127.net/68e4e99f2a0a400bfade8cd2befd0e69.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba7ed53477cc0b34a0569704be78fb7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba7ed53477cc0b34a0569704be78fb7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e1380ce14c595cc7c896ab6d80977c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e1380ce14c595cc7c896ab6d80977c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8625973becb30763b8185d5aed6ff2a.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8625973becb30763b8185d5aed6ff2a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38d2ba1a53807474d5d1908c38e44941.jpg\" _src=\"http://yanxuan.nosdn.127.net/38d2ba1a53807474d5d1908c38e44941.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19c2742c33d946ea42525bb766b9aa50.jpg\" _src=\"http://yanxuan.nosdn.127.net/19c2742c33d946ea42525bb766b9aa50.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e38f6f972d9e0a5b1b929b00dac2ab7.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e38f6f972d9e0a5b1b929b00dac2ab7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2b39cc98245fb88155269d891af0165.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2b39cc98245fb88155269d891af0165.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf6dc932f82e427196f6202d1da99fc1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf6dc932f82e427196f6202d1da99fc1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c90a23374fd5cf95dc05c0a687d52de7.jpg\" _src=\"http://yanxuan.nosdn.127.net/c90a23374fd5cf95dc05c0a687d52de7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c88e300269e108c04717dbd70539aa1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/c88e300269e108c04717dbd70539aa1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2c90271ed6fdd1b1cb114185962ac5b.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2c90271ed6fdd1b1cb114185962ac5b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/517fcab43dd3c867c9861835991185a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/517fcab43dd3c867c9861835991185a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/052b5796f383987f0982bfb21c62133d.jpg\" _src=\"http://yanxuan.nosdn.127.net/052b5796f383987f0982bfb21c62133d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/657fece964b17cdb783bce720165c81b.jpg\" _src=\"http://yanxuan.nosdn.127.net/657fece964b17cdb783bce720165c81b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3627ec2a160228289e561b4c4bad1c88.jpg\" _src=\"http://yanxuan.nosdn.127.net/3627ec2a160228289e561b4c4bad1c88.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c084cdba7d998c6026b77b2bedb16c8.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c084cdba7d998c6026b77b2bedb16c8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/609e6f0b7bcad8516f51c957c352e131.jpg\" _src=\"http://yanxuan.nosdn.127.net/609e6f0b7bcad8516f51c957c352e131.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b51e43dd314866fe7b8cf1def3896b5f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b51e43dd314866fe7b8cf1def3896b5f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f134c68159e3c4ae1b8cd31685c4a0da.jpg\" _src=\"http://yanxuan.nosdn.127.net/f134c68159e3c4ae1b8cd31685c4a0da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d6c3dd50f40ce4d2f23e33a10af02f3.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d6c3dd50f40ce4d2f23e33a10af02f3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93e670375dc312a0bce884d535b49543.jpg\" _src=\"http://yanxuan.nosdn.127.net/93e670375dc312a0bce884d535b49543.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e6ead1f50e3d5a5f7ece304975ebaf3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/e6ead1f50e3d5a5f7ece304975ebaf3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab5c9ba3fe26f2eac2908ff4ef0c3e38.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab5c9ba3fe26f2eac2908ff4ef0c3e38.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5955779f4196eacee871872e9c565237.jpg\" _src=\"http://yanxuan.nosdn.127.net/5955779f4196eacee871872e9c565237.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a54295c3a05ce118773f3b72a94ee198.jpg\" _src=\"http://yanxuan.nosdn.127.net/a54295c3a05ce118773f3b72a94ee198.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f0fb6a2b73c481dc8194efc9036daed.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f0fb6a2b73c481dc8194efc9036daed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bcffbd7e19cb83a129de0d1dcf70e3fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/bcffbd7e19cb83a129de0d1dcf70e3fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/533047cdb7474da59cb87adbe6c50e39.jpg\" _src=\"http://yanxuan.nosdn.127.net/533047cdb7474da59cb87adbe6c50e39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4aadd1564fd982d1f2267b49418441cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/4aadd1564fd982d1f2267b49418441cf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71b5a16bc159955645369c89711374c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/71b5a16bc159955645369c89711374c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19a53b3e0bbbda6ee8dc2028930371a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/19a53b3e0bbbda6ee8dc2028930371a6.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 39,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2f7641027f584b21e2f51d0a546291a0.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/30d7daa0824fbb61b6c36175c8203349.png",
      "retail_price": 559,
      "sell_volume": 22628,
      "primary_product_id": 1136431,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 1
    },
    {
      "id": 1135055,
      "category_id": 1008002,
      "goods_sn": "1135055",
      "name": "北欧印象几何条纹混色窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "山形纹提花 北欧简约混色",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/517a42ae18dfd98e7d3f311317ba3f54.jpg\" _src=\"http://yanxuan.nosdn.127.net/517a42ae18dfd98e7d3f311317ba3f54.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/68e9db2e8f912d4993a3c912e03f5f2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/68e9db2e8f912d4993a3c912e03f5f2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41bc6c237355edd4d4e8dd89c504a4b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/41bc6c237355edd4d4e8dd89c504a4b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33f3534df43afd47eb9bb9e3cb85d0b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/33f3534df43afd47eb9bb9e3cb85d0b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/304afcf82a46055f14f62da9dbf079e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/304afcf82a46055f14f62da9dbf079e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b28ab088bc909f9964ce3dc6b911439.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b28ab088bc909f9964ce3dc6b911439.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31bb168618d29b6088bfe880a99934c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/31bb168618d29b6088bfe880a99934c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d965a3607b1a22f7f52e01261d7a507b.jpg\" _src=\"http://yanxuan.nosdn.127.net/d965a3607b1a22f7f52e01261d7a507b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f868badfd66ad1ed70fb7abc4a71f5b.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f868badfd66ad1ed70fb7abc4a71f5b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/662697d3bcdb8427452aec321d3e4c6a.jpg\" _src=\"http://yanxuan.nosdn.127.net/662697d3bcdb8427452aec321d3e4c6a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cdf2fd88a844f539f4c9873efb14a93d.jpg\" _src=\"http://yanxuan.nosdn.127.net/cdf2fd88a844f539f4c9873efb14a93d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1792cab519f6f0b489ddf95c30023f67.jpg\" _src=\"http://yanxuan.nosdn.127.net/1792cab519f6f0b489ddf95c30023f67.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/334801d2a30855b7bf207bf295b4ecfc.jpg\" _src=\"http://yanxuan.nosdn.127.net/334801d2a30855b7bf207bf295b4ecfc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c18a7d948ec0ed09d777291a5f547ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c18a7d948ec0ed09d777291a5f547ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9bc0be56147bf743458d8df50fc5075f.jpg\" _src=\"http://yanxuan.nosdn.127.net/9bc0be56147bf743458d8df50fc5075f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f89950e36bc4c8ac8cb53e6b4377a9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f89950e36bc4c8ac8cb53e6b4377a9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3322ca38b778f0a9b3ac20a049cf520d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3322ca38b778f0a9b3ac20a049cf520d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa487adfab5d685e9da06822a2ea5bb9.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa487adfab5d685e9da06822a2ea5bb9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23425bf14b340a87dcc22c9c4390e15e.jpg\" _src=\"http://yanxuan.nosdn.127.net/23425bf14b340a87dcc22c9c4390e15e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f1e82fc020816d3eb2ef17e24b9e5d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f1e82fc020816d3eb2ef17e24b9e5d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba7a8e956add1c16e9e49ca0d72bd30e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba7a8e956add1c16e9e49ca0d72bd30e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21635d8fed07731fe9d6e5a74bc69c41.jpg\" _src=\"http://yanxuan.nosdn.127.net/21635d8fed07731fe9d6e5a74bc69c41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ed0d59cbd62397d20b5fbf4626d41a93.jpg\" _src=\"http://yanxuan.nosdn.127.net/ed0d59cbd62397d20b5fbf4626d41a93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29d5b386af4b5f6a03996655d8295bae.jpg\" _src=\"http://yanxuan.nosdn.127.net/29d5b386af4b5f6a03996655d8295bae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0843c621c7f7d0d36cebcc5a1caf5d94.jpg\" _src=\"http://yanxuan.nosdn.127.net/0843c621c7f7d0d36cebcc5a1caf5d94.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bcb983612a08f762bd3bcc42dc98c709.jpg\" _src=\"http://yanxuan.nosdn.127.net/bcb983612a08f762bd3bcc42dc98c709.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7fe59f3d9cda66b0fd4a2c94e124d0ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/7fe59f3d9cda66b0fd4a2c94e124d0ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31bd379ac7037b5e54ea93e4f8f833e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/31bd379ac7037b5e54ea93e4f8f833e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/331051a617e47532461c31e5ff7a16bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/331051a617e47532461c31e5ff7a16bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/443cd3bba1bc4e24a17801750b8ffd73.jpg\" _src=\"http://yanxuan.nosdn.127.net/443cd3bba1bc4e24a17801750b8ffd73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b408464b2167c203bd691c80badedeae.jpg\" _src=\"http://yanxuan.nosdn.127.net/b408464b2167c203bd691c80badedeae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79107afd183d1fe4429dd84e27b1869c.jpg\" _src=\"http://yanxuan.nosdn.127.net/79107afd183d1fe4429dd84e27b1869c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dcd5d9008ff6dbc93631ce29dab6b354.jpg\" _src=\"http://yanxuan.nosdn.127.net/dcd5d9008ff6dbc93631ce29dab6b354.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5f53f0045b4a770124615a12e724ced.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5f53f0045b4a770124615a12e724ced.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25ddf1a21d8d5a43ab3b1a5d505c65d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/25ddf1a21d8d5a43ab3b1a5d505c65d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbf4143559b00939a44fde123c8c2888.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbf4143559b00939a44fde123c8c2888.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2dac797df342a33a30e45e365ccbbfd9.jpg\" _src=\"http://yanxuan.nosdn.127.net/2dac797df342a33a30e45e365ccbbfd9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8c2564a0a643c338a3ba3ca6c7e7ff58.jpg\" _src=\"http://yanxuan.nosdn.127.net/8c2564a0a643c338a3ba3ca6c7e7ff58.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19cc6dc4032ac9ce30325fc92a5e345e.jpg\" _src=\"http://yanxuan.nosdn.127.net/19cc6dc4032ac9ce30325fc92a5e345e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb623f2b464c8cec997dc021a89571b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb623f2b464c8cec997dc021a89571b9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5bb40f61105e0380f7fec424ca29b1fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/5bb40f61105e0380f7fec424ca29b1fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/344edfec8435287400477554e2a4fcba.jpg\" _src=\"http://yanxuan.nosdn.127.net/344edfec8435287400477554e2a4fcba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9f33ab114476550b418a3f0fbaeea68.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9f33ab114476550b418a3f0fbaeea68.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b72c8e0a58bd04c363306fbd3bf429df.jpg\" _src=\"http://yanxuan.nosdn.127.net/b72c8e0a58bd04c363306fbd3bf429df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6a7308307c74336da7ff7330436a3dd6.jpg\" _src=\"http://yanxuan.nosdn.127.net/6a7308307c74336da7ff7330436a3dd6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b1086c39d44b373a2e8cdb3062d8c30.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b1086c39d44b373a2e8cdb3062d8c30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c95781a9b95d7e01d384b410cb7a6a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c95781a9b95d7e01d384b410cb7a6a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd1f991f3beb2d9861df203c22a03b08.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd1f991f3beb2d9861df203c22a03b08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a55eccfd7e14fea5c551be5b94bf8851.jpg\" _src=\"http://yanxuan.nosdn.127.net/a55eccfd7e14fea5c551be5b94bf8851.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af209f2726ee582a11b0adf4473963bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/af209f2726ee582a11b0adf4473963bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb4b661f960dfab272a833732a338b84.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb4b661f960dfab272a833732a338b84.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0eac0f1694749e3f2ba7c3ce73234ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0eac0f1694749e3f2ba7c3ce73234ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9817135b6416cc72642ada8d285a22d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9817135b6416cc72642ada8d285a22d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54443af2a33be3579ecfff18eeabb321.jpg\" _src=\"http://yanxuan.nosdn.127.net/54443af2a33be3579ecfff18eeabb321.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f79c86438c27c8c0ad9511683fb900c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f79c86438c27c8c0ad9511683fb900c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebdc8e8f06f2fbe11bc2765038906df7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebdc8e8f06f2fbe11bc2765038906df7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e2cb3235a86089e75b3b848af26755e.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e2cb3235a86089e75b3b848af26755e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2fef8703070e9b1be2e1367bb7c8ea00.jpg\" _src=\"http://yanxuan.nosdn.127.net/2fef8703070e9b1be2e1367bb7c8ea00.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c84eb4b1c7bb644faf451da2e2b0447.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c84eb4b1c7bb644faf451da2e2b0447.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7df41298392f5c0f38965e2b2097178a.jpg\" _src=\"http://yanxuan.nosdn.127.net/7df41298392f5c0f38965e2b2097178a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d458e8bf25e7c2877ed2b1ef5637aa9.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d458e8bf25e7c2877ed2b1ef5637aa9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/98cbb394e2b1cae7aaa848c85dd3af18.jpg\" _src=\"http://yanxuan.nosdn.127.net/98cbb394e2b1cae7aaa848c85dd3af18.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e162e4742a0865e047b3e189591ae8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e162e4742a0865e047b3e189591ae8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4dfd24919e00f6c0715ce2323507c935.jpg\" _src=\"http://yanxuan.nosdn.127.net/4dfd24919e00f6c0715ce2323507c935.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/202ad04b025d49988cc0b4cabcca70f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/202ad04b025d49988cc0b4cabcca70f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b72277b67793dc6542783a2d0973869.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b72277b67793dc6542783a2d0973869.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75bceb04c01f9ebbe533a94b5eccb873.jpg\" _src=\"http://yanxuan.nosdn.127.net/75bceb04c01f9ebbe533a94b5eccb873.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/465b9fc2f115f3881e90120c738ece73.jpg\" _src=\"http://yanxuan.nosdn.127.net/465b9fc2f115f3881e90120c738ece73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/66dfd8708bd9d6ec229f56d22d1f1e82.jpg\" _src=\"http://yanxuan.nosdn.127.net/66dfd8708bd9d6ec229f56d22d1f1e82.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 37,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/0db87bc9137f5ca00f0d2de15a7cf607.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/87b6a608b99279ebf1764682e9e5fcec.png",
      "retail_price": 399,
      "sell_volume": 17157,
      "primary_product_id": 1136456,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135056,
      "category_id": 1008002,
      "goods_sn": "1135056",
      "name": "糖果色凹凸条纹儿童房窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "灵动色彩，童趣条纹",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/7c20355c62ad66dbba32b0e11f0f75d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c20355c62ad66dbba32b0e11f0f75d5.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35552ca10129c4ec6530fbd5b3596f5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/35552ca10129c4ec6530fbd5b3596f5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba98905fc96c69c0a4bf4caec083be2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba98905fc96c69c0a4bf4caec083be2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08f9e46394d65290533db13e32112890.jpg\" _src=\"http://yanxuan.nosdn.127.net/08f9e46394d65290533db13e32112890.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b16ba0cc72ef435e2999564ec20cf6c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b16ba0cc72ef435e2999564ec20cf6c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/df3a97cb4c73bc9c1036bb0446368630.jpg\" _src=\"http://yanxuan.nosdn.127.net/df3a97cb4c73bc9c1036bb0446368630.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c6505b769f5c54f6e66231b03d9c9919.jpg\" _src=\"http://yanxuan.nosdn.127.net/c6505b769f5c54f6e66231b03d9c9919.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59a6179c8b6f523bc6c67646fcf0ca08.jpg\" _src=\"http://yanxuan.nosdn.127.net/59a6179c8b6f523bc6c67646fcf0ca08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3b4ce480059631e26ffac109aa5d18c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3b4ce480059631e26ffac109aa5d18c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/57dbe2baf75e5fa5529d1b3fd0ebdc97.jpg\" _src=\"http://yanxuan.nosdn.127.net/57dbe2baf75e5fa5529d1b3fd0ebdc97.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/72b5df8ead55acb75c626b7c4f22f76d.jpg\" _src=\"http://yanxuan.nosdn.127.net/72b5df8ead55acb75c626b7c4f22f76d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a34c76a1a5bd369b0c7acf62813746a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a34c76a1a5bd369b0c7acf62813746a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c9fb571be38cc011c8edbaff7ab7c961.jpg\" _src=\"http://yanxuan.nosdn.127.net/c9fb571be38cc011c8edbaff7ab7c961.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae2f00a619449bbc968efbb99a0aacfd.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae2f00a619449bbc968efbb99a0aacfd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fe6dabb85692fd165279f626a27f9fb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/fe6dabb85692fd165279f626a27f9fb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f0e4d2016335e408106495abc2cf925.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f0e4d2016335e408106495abc2cf925.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfd6f2404e14e54f45f26baff796fca9.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfd6f2404e14e54f45f26baff796fca9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a034ad41437cb22dc27edeb8c7ced17c.jpg\" _src=\"http://yanxuan.nosdn.127.net/a034ad41437cb22dc27edeb8c7ced17c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d73f789cd190aaaf80d426939bfc4466.jpg\" _src=\"http://yanxuan.nosdn.127.net/d73f789cd190aaaf80d426939bfc4466.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a375c717468e02d130a3b335a469b4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a375c717468e02d130a3b335a469b4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3160e6ae5c4e0cf4809b0d7419c3bf5.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3160e6ae5c4e0cf4809b0d7419c3bf5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0f8b77d9f28c35569d92d18f72c8c27.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0f8b77d9f28c35569d92d18f72c8c27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b613b3604ded989f3aaeb1b3af5e7c60.jpg\" _src=\"http://yanxuan.nosdn.127.net/b613b3604ded989f3aaeb1b3af5e7c60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82d1d397861c98813e93876f878ed02a.jpg\" _src=\"http://yanxuan.nosdn.127.net/82d1d397861c98813e93876f878ed02a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/628c2aa615c30a97b2c43d829b75161f.jpg\" _src=\"http://yanxuan.nosdn.127.net/628c2aa615c30a97b2c43d829b75161f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/01899c4632878aa07b12e74b67259485.jpg\" _src=\"http://yanxuan.nosdn.127.net/01899c4632878aa07b12e74b67259485.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82554461e3615eea2564fbb9290e57ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/82554461e3615eea2564fbb9290e57ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/36b38aca196c62338811f878e18f52b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/36b38aca196c62338811f878e18f52b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a27d72b8fe9e3d533c8c448f7b4a0614.jpg\" _src=\"http://yanxuan.nosdn.127.net/a27d72b8fe9e3d533c8c448f7b4a0614.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e68d027072ddbb0420b21e3f0f44365.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e68d027072ddbb0420b21e3f0f44365.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c62bd7b6ce6ee1da5a27062df9363677.jpg\" _src=\"http://yanxuan.nosdn.127.net/c62bd7b6ce6ee1da5a27062df9363677.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76fde5b8b397c0efb12685fd8561123d.jpg\" _src=\"http://yanxuan.nosdn.127.net/76fde5b8b397c0efb12685fd8561123d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5816b3d9fae2b1d15fc462729fe977d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5816b3d9fae2b1d15fc462729fe977d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d57f643c8d33996708bab3052144aa99.jpg\" _src=\"http://yanxuan.nosdn.127.net/d57f643c8d33996708bab3052144aa99.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ecf67d3847b9050a377f751ce250ce34.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecf67d3847b9050a377f751ce250ce34.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e01c7dc028bedd59001e7345a5a246d.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e01c7dc028bedd59001e7345a5a246d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4662d564c3b6df760dd19139a6af3060.jpg\" _src=\"http://yanxuan.nosdn.127.net/4662d564c3b6df760dd19139a6af3060.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2bab03382de1776e2cb9021947f44807.jpg\" _src=\"http://yanxuan.nosdn.127.net/2bab03382de1776e2cb9021947f44807.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/668e0c4505f9b86190207fe0d8be84ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/668e0c4505f9b86190207fe0d8be84ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19dbde9ef6edf5c1c8790049662287df.jpg\" _src=\"http://yanxuan.nosdn.127.net/19dbde9ef6edf5c1c8790049662287df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53464274e000ef9c108a6875a4dc7a4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/53464274e000ef9c108a6875a4dc7a4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/138ff2f3f471cf84169a16730ac61c1a.jpg\" _src=\"http://yanxuan.nosdn.127.net/138ff2f3f471cf84169a16730ac61c1a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1397ec9bc1f099328c4991b1e1ba224d.jpg\" _src=\"http://yanxuan.nosdn.127.net/1397ec9bc1f099328c4991b1e1ba224d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15ea2d7f9648e1e40915d3e300411994.jpg\" _src=\"http://yanxuan.nosdn.127.net/15ea2d7f9648e1e40915d3e300411994.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3011b59e959f2ef7f4ce50960b45af9c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3011b59e959f2ef7f4ce50960b45af9c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e74c96c5e3bb615176591afbb20d5b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e74c96c5e3bb615176591afbb20d5b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fe8022ad7a0af1a1d3fd775789b43871.jpg\" _src=\"http://yanxuan.nosdn.127.net/fe8022ad7a0af1a1d3fd775789b43871.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb33363454d749da01e88d7f33d47637.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb33363454d749da01e88d7f33d47637.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b57a6785a7ca57472ead814b5e663ed9.jpg\" _src=\"http://yanxuan.nosdn.127.net/b57a6785a7ca57472ead814b5e663ed9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/58338bfd632396d37a32cc3a111e6d42.jpg\" _src=\"http://yanxuan.nosdn.127.net/58338bfd632396d37a32cc3a111e6d42.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f3d6d7f4d4e9fd6d4b7199ec3f993056.jpg\" _src=\"http://yanxuan.nosdn.127.net/f3d6d7f4d4e9fd6d4b7199ec3f993056.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e1bd19661b084036aef793cd04eb850.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e1bd19661b084036aef793cd04eb850.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a4a7ec58407e2c179a268c5f7d9f71b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a4a7ec58407e2c179a268c5f7d9f71b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b752ea0fa16847a196c7c72f9b3c790.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b752ea0fa16847a196c7c72f9b3c790.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2b901ebaf68371b049d87036eb8f41f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2b901ebaf68371b049d87036eb8f41f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f700d302dfb86c98afc8655526129c05.jpg\" _src=\"http://yanxuan.nosdn.127.net/f700d302dfb86c98afc8655526129c05.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb322b63a80aa3e44cca7d0c8fb06820.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb322b63a80aa3e44cca7d0c8fb06820.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d89b92178625b1c87406c1406c891aa7.jpg\" _src=\"http://yanxuan.nosdn.127.net/d89b92178625b1c87406c1406c891aa7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2e4a0c0718ab1f434af40220649c4776.jpg\" _src=\"http://yanxuan.nosdn.127.net/2e4a0c0718ab1f434af40220649c4776.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8cab72015ab23ae571eb8deb0f688870.jpg\" _src=\"http://yanxuan.nosdn.127.net/8cab72015ab23ae571eb8deb0f688870.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f9db276e7c5b8f81223da9bf2b81d146.jpg\" _src=\"http://yanxuan.nosdn.127.net/f9db276e7c5b8f81223da9bf2b81d146.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e026d4db4dbdb745a970db7aab7a5ff.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e026d4db4dbdb745a970db7aab7a5ff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abb53b015f71f95844b9b645f8d2a28e.jpg\" _src=\"http://yanxuan.nosdn.127.net/abb53b015f71f95844b9b645f8d2a28e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fae009fcecbb3b4d387519524f991457.jpg\" _src=\"http://yanxuan.nosdn.127.net/fae009fcecbb3b4d387519524f991457.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/05827553784f26cf0ccc6b02c3b1c7dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/05827553784f26cf0ccc6b02c3b1c7dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16d0bf68cd235dac5b72f47d4c7ace7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/16d0bf68cd235dac5b72f47d4c7ace7f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db55ff3fe3873426c8d047d3403387cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/db55ff3fe3873426c8d047d3403387cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/df067a032a8e3f85b7b1e9f3ae4a0ed6.jpg\" _src=\"http://yanxuan.nosdn.127.net/df067a032a8e3f85b7b1e9f3ae4a0ed6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a39eaca1d201e2f71f28c4ffa339e87a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a39eaca1d201e2f71f28c4ffa339e87a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f9ff903bc8538e43ba0de5fcd57c3e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f9ff903bc8538e43ba0de5fcd57c3e2.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 36,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/5b9da3d72c73da202972f88ee1c7837b.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/536246ca4adb77274a94b18bb2f91f47.png",
      "retail_price": 259,
      "sell_volume": 10577,
      "primary_product_id": 1136472,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135057,
      "category_id": 1008002,
      "goods_sn": "1135057",
      "name": "梦幻系简约轻透莹白纱帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "轻透柔软纱 朦胧细纹肌理",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/088e63e0e298739ce0b7ad6aa4f3bc2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/088e63e0e298739ce0b7ad6aa4f3bc2d.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44d08314b0c25796e5211b7f82d9c9cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/44d08314b0c25796e5211b7f82d9c9cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7a2aede16ff390bc980e8bd485e4e6a.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7a2aede16ff390bc980e8bd485e4e6a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb015656f9c0cf779739438143c7842d.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb015656f9c0cf779739438143c7842d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a76c38ce3e756deba85a09fe5551abcd.jpg\" _src=\"http://yanxuan.nosdn.127.net/a76c38ce3e756deba85a09fe5551abcd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f15917590cd0a049c095a2c95ccf832a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f15917590cd0a049c095a2c95ccf832a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1905c8981f963198da77643f3f774a54.jpg\" _src=\"http://yanxuan.nosdn.127.net/1905c8981f963198da77643f3f774a54.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2ccdfcf68dd4c0f908cfa5c48c76e3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2ccdfcf68dd4c0f908cfa5c48c76e3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae6093e376c8ce4b008e5eef96cd2f6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae6093e376c8ce4b008e5eef96cd2f6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5c6b8de674a14425396608d1788a6bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5c6b8de674a14425396608d1788a6bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa9780ed9a8e1a744c589005428eccb3.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa9780ed9a8e1a744c589005428eccb3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/814d1ee43b10292e38a838e32242ff95.jpg\" _src=\"http://yanxuan.nosdn.127.net/814d1ee43b10292e38a838e32242ff95.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbbe9bb7409bbc29285394c56fe6de65.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbbe9bb7409bbc29285394c56fe6de65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/001bc932cab905300c5c00a6da69db28.jpg\" _src=\"http://yanxuan.nosdn.127.net/001bc932cab905300c5c00a6da69db28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8bb1b60c6a52683d4d2689894ccbf20.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8bb1b60c6a52683d4d2689894ccbf20.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/817206ab2ffd7946e99f2c459bb725ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/817206ab2ffd7946e99f2c459bb725ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/557da67f50abfebb9f38c066ab7b202c.jpg\" _src=\"http://yanxuan.nosdn.127.net/557da67f50abfebb9f38c066ab7b202c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf68d5bcaba0405d7a3043f7ea36663a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf68d5bcaba0405d7a3043f7ea36663a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/195cc13edfaaafa97d8f836e5d1c841a.jpg\" _src=\"http://yanxuan.nosdn.127.net/195cc13edfaaafa97d8f836e5d1c841a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27757a632a1b76e68b1ac520a2bfd5a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/27757a632a1b76e68b1ac520a2bfd5a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c24fe54ae36bd45b741a5ba8796113a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c24fe54ae36bd45b741a5ba8796113a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/894a5ae76c69eb6759de91212a83fa04.jpg\" _src=\"http://yanxuan.nosdn.127.net/894a5ae76c69eb6759de91212a83fa04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b3aca05774b786d461645ec4faeefda.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b3aca05774b786d461645ec4faeefda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37293874fef9660e431fbe5d2f0a1fad.jpg\" _src=\"http://yanxuan.nosdn.127.net/37293874fef9660e431fbe5d2f0a1fad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3f6bb62defe913a888f049be018daa0.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3f6bb62defe913a888f049be018daa0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35d2a4c32aa83b360cf60cb6a6c71d8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/35d2a4c32aa83b360cf60cb6a6c71d8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6758ccc43d3a31997bcdfedad718f6e3.jpg\" _src=\"http://yanxuan.nosdn.127.net/6758ccc43d3a31997bcdfedad718f6e3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d101a311f94525444c79075e6dc8a90f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d101a311f94525444c79075e6dc8a90f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d336e42a2f94454ce0078be4389d4b2.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d336e42a2f94454ce0078be4389d4b2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dae266d530a47edde62a0424b49cfe73.jpg\" _src=\"http://yanxuan.nosdn.127.net/dae266d530a47edde62a0424b49cfe73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c2d1071f14177b19d292b6887544d6e.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c2d1071f14177b19d292b6887544d6e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e027ee3bc3fa0ced129d05dd85f629a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e027ee3bc3fa0ced129d05dd85f629a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5c56b8c566ae2dcc0697b4e7bb8b8630.jpg\" _src=\"http://yanxuan.nosdn.127.net/5c56b8c566ae2dcc0697b4e7bb8b8630.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be84eaf810654923eb06310883435942.jpg\" _src=\"http://yanxuan.nosdn.127.net/be84eaf810654923eb06310883435942.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b207cfccb4eda5a7278bd74c82adacda.jpg\" _src=\"http://yanxuan.nosdn.127.net/b207cfccb4eda5a7278bd74c82adacda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54f86d151cf250d3a76a4cd725f9cdfe.jpg\" _src=\"http://yanxuan.nosdn.127.net/54f86d151cf250d3a76a4cd725f9cdfe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44d3695e8dd5286b029aa7ce19a5b97a.jpg\" _src=\"http://yanxuan.nosdn.127.net/44d3695e8dd5286b029aa7ce19a5b97a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c80a2af6d1d1b40d382b1f495e83795.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c80a2af6d1d1b40d382b1f495e83795.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddd6008d180e884835cfd39094a81dd7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddd6008d180e884835cfd39094a81dd7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b70b0bbb4933b57f7d28f517ef9c812.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b70b0bbb4933b57f7d28f517ef9c812.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/251f9ccb814f04ca5e6804b5ca60182f.jpg\" _src=\"http://yanxuan.nosdn.127.net/251f9ccb814f04ca5e6804b5ca60182f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad8ca0f8ffd3396ee1be6792b316d8fb.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad8ca0f8ffd3396ee1be6792b316d8fb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/96237772643462f0c923051df580ef8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/96237772643462f0c923051df580ef8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/054f71961df4fca4c0260d83a5d9bc98.jpg\" _src=\"http://yanxuan.nosdn.127.net/054f71961df4fca4c0260d83a5d9bc98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d5cbcffbfcd3ac01e38eb3a01d0833a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/d5cbcffbfcd3ac01e38eb3a01d0833a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb4bb9f35b500e7a0a7093ddbce407f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb4bb9f35b500e7a0a7093ddbce407f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23a6091b704260334779826d2b858a9f.jpg\" _src=\"http://yanxuan.nosdn.127.net/23a6091b704260334779826d2b858a9f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aec34514179b3837429f6e4ab9f39759.jpg\" _src=\"http://yanxuan.nosdn.127.net/aec34514179b3837429f6e4ab9f39759.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/339a771531698027d36f917ccafadd02.jpg\" _src=\"http://yanxuan.nosdn.127.net/339a771531698027d36f917ccafadd02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/06def276699cc40e8f281c1f0b935c04.jpg\" _src=\"http://yanxuan.nosdn.127.net/06def276699cc40e8f281c1f0b935c04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2648155e986745bf2269ef0857968bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2648155e986745bf2269ef0857968bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ef7a8e1db5aceba36645696895b04671.jpg\" _src=\"http://yanxuan.nosdn.127.net/ef7a8e1db5aceba36645696895b04671.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddb0d7fee5bde51071746aef961e28d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddb0d7fee5bde51071746aef961e28d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6752bad820840f5f0b684690d35f697d.jpg\" _src=\"http://yanxuan.nosdn.127.net/6752bad820840f5f0b684690d35f697d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaec96a0239f848e38d79510191480a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaec96a0239f848e38d79510191480a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad7d5c557d09e854388d33963566712e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad7d5c557d09e854388d33963566712e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d64a872b7b803ae2c6a3342edae85bb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/d64a872b7b803ae2c6a3342edae85bb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/859f290857188c448bdca0e20cf786ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/859f290857188c448bdca0e20cf786ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6cc76f812f3a2ebc107cc3d5e0c8da75.jpg\" _src=\"http://yanxuan.nosdn.127.net/6cc76f812f3a2ebc107cc3d5e0c8da75.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 33,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a007b270ec16a4d4c2c9e18d3b5cb06b.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/98c5e80b8e328687ce9c949314ebc41d.png",
      "retail_price": 199,
      "sell_volume": 4968,
      "primary_product_id": 1136484,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135058,
      "category_id": 1008002,
      "goods_sn": "1135058",
      "name": "日式多功能手卷午睡枕坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "全棉针织条纹，透气按摩粒子",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/2286fb6b29d365466760ecbf2ebc8c82.jpg\" _src=\"http://yanxuan.nosdn.127.net/2286fb6b29d365466760ecbf2ebc8c82.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9b2bd6e1049c5c4653a00b9802e6a11.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9b2bd6e1049c5c4653a00b9802e6a11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2639883802a55490ea81fe3dcd543df3.jpg\" _src=\"http://yanxuan.nosdn.127.net/2639883802a55490ea81fe3dcd543df3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/582b3658d2e405bd74dce301502d70f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/582b3658d2e405bd74dce301502d70f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba9df33cbb0003bdab7d63dd0a70d599.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba9df33cbb0003bdab7d63dd0a70d599.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/24c5d1905d9c31072445d87f7a37eebb.jpg\" _src=\"http://yanxuan.nosdn.127.net/24c5d1905d9c31072445d87f7a37eebb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e874eec46f85b846f696dd11fe61b858.jpg\" _src=\"http://yanxuan.nosdn.127.net/e874eec46f85b846f696dd11fe61b858.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d64ae710b7fc2c1cef03d7582515ede0.jpg\" _src=\"http://yanxuan.nosdn.127.net/d64ae710b7fc2c1cef03d7582515ede0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab294e2889662c548e3e283e548d7ca2.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab294e2889662c548e3e283e548d7ca2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2eb3eaef8f70960e95c67048faf1c68c.jpg\" _src=\"http://yanxuan.nosdn.127.net/2eb3eaef8f70960e95c67048faf1c68c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11bf7eb8c196ecc361c963836b81d4ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/11bf7eb8c196ecc361c963836b81d4ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ef7b28262d2d7def40175ca98bde3222.jpg\" _src=\"http://yanxuan.nosdn.127.net/ef7b28262d2d7def40175ca98bde3222.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/678ae536ac582a2923cfa8240bf66aa8.jpg\" _src=\"http://yanxuan.nosdn.127.net/678ae536ac582a2923cfa8240bf66aa8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32d157099c01a5c6283513849f699d0f.jpg\" _src=\"http://yanxuan.nosdn.127.net/32d157099c01a5c6283513849f699d0f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e74c91fa555929d5493dcde5da877b02.jpg\" _src=\"http://yanxuan.nosdn.127.net/e74c91fa555929d5493dcde5da877b02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e511841b236e95ab4ff0bf4562500ad0.jpg\" _src=\"http://yanxuan.nosdn.127.net/e511841b236e95ab4ff0bf4562500ad0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/deb067ad58dea4f11f53b191e3d1e77f.jpg\" _src=\"http://yanxuan.nosdn.127.net/deb067ad58dea4f11f53b191e3d1e77f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76a6d1fc324d373f70db08ce8750cb32.jpg\" _src=\"http://yanxuan.nosdn.127.net/76a6d1fc324d373f70db08ce8750cb32.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6305c83e95ddddd661cef3d5c9ac58cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6305c83e95ddddd661cef3d5c9ac58cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c9dcf3269c87105f1841aed22d0f36fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/c9dcf3269c87105f1841aed22d0f36fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54d7c9813569e17cef0f1027e5a52e6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/54d7c9813569e17cef0f1027e5a52e6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d39f00c7e20a5cd1a9ee8c9a65744cc0.jpg\" _src=\"http://yanxuan.nosdn.127.net/d39f00c7e20a5cd1a9ee8c9a65744cc0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3bcd9d4b95c77f2a61dc5e29cd804cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3bcd9d4b95c77f2a61dc5e29cd804cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f52a276d2daf93cb61be8d6b6509106a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f52a276d2daf93cb61be8d6b6509106a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d659bfb20371020a769309886aadd16f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d659bfb20371020a769309886aadd16f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/43d05684abd3de808a8e35506a232c76.jpg\" _src=\"http://yanxuan.nosdn.127.net/43d05684abd3de808a8e35506a232c76.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48905901467d7f0950220b3eac766519.jpg\" _src=\"http://yanxuan.nosdn.127.net/48905901467d7f0950220b3eac766519.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ed5dcbd0e5d8b53cd6c4116780415af.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ed5dcbd0e5d8b53cd6c4116780415af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f0e8dbe1a4acb9985534c1a1017b91ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/f0e8dbe1a4acb9985534c1a1017b91ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5953f2c981375ea3945f368b9efcf2e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/5953f2c981375ea3945f368b9efcf2e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2afc692ecef8565da94ab96d605bd8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2afc692ecef8565da94ab96d605bd8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1c74ac52f6858cbaf6795bb98269a60.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1c74ac52f6858cbaf6795bb98269a60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c1090b13b82a36d182644a78c1ade112.jpg\" _src=\"http://yanxuan.nosdn.127.net/c1090b13b82a36d182644a78c1ade112.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d28fba7b538217405ad66fb119e5fa0.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d28fba7b538217405ad66fb119e5fa0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22588b3bc32226a798cb1ae6106525ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/22588b3bc32226a798cb1ae6106525ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9f07dcfdfa0e7a90df6e8c9ea397d17.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9f07dcfdfa0e7a90df6e8c9ea397d17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/00df39022e7a1c29a9c0fbf4a0e3fb38.jpg\" _src=\"http://yanxuan.nosdn.127.net/00df39022e7a1c29a9c0fbf4a0e3fb38.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8588aabc1bbe4475026d74052b166a51.jpg\" _src=\"http://yanxuan.nosdn.127.net/8588aabc1bbe4475026d74052b166a51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22071588ec58dfd880e913908acf2544.jpg\" _src=\"http://yanxuan.nosdn.127.net/22071588ec58dfd880e913908acf2544.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8f02bcd66829318d9ca39618df2f42f.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8f02bcd66829318d9ca39618df2f42f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0a72a74333e658a4da4bf886d74d739.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0a72a74333e658a4da4bf886d74d739.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e40a7ae5c9834f61408a1d31c839d79.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e40a7ae5c9834f61408a1d31c839d79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af4812a2debd12fb561816f2df84fddc.jpg\" _src=\"http://yanxuan.nosdn.127.net/af4812a2debd12fb561816f2df84fddc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e8182e35711a99d7e443bd69908948e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/e8182e35711a99d7e443bd69908948e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82ca0181ca502c76834e528135b272e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/82ca0181ca502c76834e528135b272e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f359915790a2bc8a399f243357da1cd4.jpg\" _src=\"http://yanxuan.nosdn.127.net/f359915790a2bc8a399f243357da1cd4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa9246460b556890c5fdd5a8cc305743.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa9246460b556890c5fdd5a8cc305743.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5381c329f434e08e18e087ebec952a28.jpg\" _src=\"http://yanxuan.nosdn.127.net/5381c329f434e08e18e087ebec952a28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f966701c7b93490c5cebf8e9cfdffa5.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f966701c7b93490c5cebf8e9cfdffa5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/056d111c415c9db7282d8a27aeed9ae8.jpg\" _src=\"http://yanxuan.nosdn.127.net/056d111c415c9db7282d8a27aeed9ae8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32dc1dbca7a4922e8da3aaf90ca5f1be.jpg\" _src=\"http://yanxuan.nosdn.127.net/32dc1dbca7a4922e8da3aaf90ca5f1be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ca114e5755a30f1557f8c75b89b1902.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ca114e5755a30f1557f8c75b89b1902.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/959c4385428233e4ec256a6646ced133.jpg\" _src=\"http://yanxuan.nosdn.127.net/959c4385428233e4ec256a6646ced133.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 16,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/56fe8e4eda700613d852141b0fd22fa1.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/37bc0fa3524a904ac740340fa92bd515.png",
      "retail_price": 79,
      "sell_volume": 2023,
      "primary_product_id": 1136490,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1138000,
      "category_id": 1008002,
      "goods_sn": "1138000",
      "name": "日式蓬软太鼓抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "萌趣太鼓造型 软糯轻柔回弹",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/c0433bd3aafdc44b2b5fe10ced151823.jpg\" _src=\"http://yanxuan.nosdn.127.net/c0433bd3aafdc44b2b5fe10ced151823.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/241526b14e760f3b327d745127b7cadd.jpg\" _src=\"http://yanxuan.nosdn.127.net/241526b14e760f3b327d745127b7cadd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/924f6a3a78957b404ea2ad0ea24b4d58.jpg\" _src=\"http://yanxuan.nosdn.127.net/924f6a3a78957b404ea2ad0ea24b4d58.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21b519690bf5574c6a4794fd0663fa37.jpg\" _src=\"http://yanxuan.nosdn.127.net/21b519690bf5574c6a4794fd0663fa37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40ce0f2d0f0331024cb5eeffd48613f5.jpg\" _src=\"http://yanxuan.nosdn.127.net/40ce0f2d0f0331024cb5eeffd48613f5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/707d4c2e44903802f5181edc4d5e2aa4.jpg\" _src=\"http://yanxuan.nosdn.127.net/707d4c2e44903802f5181edc4d5e2aa4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0a26d87e0542007a59158a814b999f67.jpg\" _src=\"http://yanxuan.nosdn.127.net/0a26d87e0542007a59158a814b999f67.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5732b17001835e524acac7d3b75685e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/5732b17001835e524acac7d3b75685e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19a4e7e34b7507e1ffb7ff3a3939a0fe.jpg\" _src=\"http://yanxuan.nosdn.127.net/19a4e7e34b7507e1ffb7ff3a3939a0fe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/699bf4c433ba2bb7736401e2272a2697.jpg\" _src=\"http://yanxuan.nosdn.127.net/699bf4c433ba2bb7736401e2272a2697.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb28a8cb46ffd42a39122d3f0724b3ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb28a8cb46ffd42a39122d3f0724b3ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/43f3eeb3661f54db929a9e3c8ee8be1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/43f3eeb3661f54db929a9e3c8ee8be1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37b4e61572b7c69462ae74b6a3cb4cb3.jpg\" _src=\"http://yanxuan.nosdn.127.net/37b4e61572b7c69462ae74b6a3cb4cb3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd17986d401a93b01526b7855e722efa.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd17986d401a93b01526b7855e722efa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e76a0c72a3e6cc2f15f61048ef1423c8.jpg\" _src=\"http://yanxuan.nosdn.127.net/e76a0c72a3e6cc2f15f61048ef1423c8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eabbdb77f25b449b1b3bcfd740a5c85c.jpg\" _src=\"http://yanxuan.nosdn.127.net/eabbdb77f25b449b1b3bcfd740a5c85c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c92f5747f156e0c3df3873456bfdc364.jpg\" _src=\"http://yanxuan.nosdn.127.net/c92f5747f156e0c3df3873456bfdc364.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fce1bbb0804c45fcedc0d407526197bd.jpg\" _src=\"http://yanxuan.nosdn.127.net/fce1bbb0804c45fcedc0d407526197bd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de893522b3454e6769d46d5d16c35ec9.jpg\" _src=\"http://yanxuan.nosdn.127.net/de893522b3454e6769d46d5d16c35ec9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c7ca459ec92d9f32b25c4d1681a3efdf.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7ca459ec92d9f32b25c4d1681a3efdf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd7974a599497d0830fe209f572f1d43.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd7974a599497d0830fe209f572f1d43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a52672cac9385c1a6da086e46aead878.jpg\" _src=\"http://yanxuan.nosdn.127.net/a52672cac9385c1a6da086e46aead878.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/edc7589ef8d2d748b10d4fbe62d6cad9.jpg\" _src=\"http://yanxuan.nosdn.127.net/edc7589ef8d2d748b10d4fbe62d6cad9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/769529f68aad47685e9fd8ccc88a5065.jpg\" _src=\"http://yanxuan.nosdn.127.net/769529f68aad47685e9fd8ccc88a5065.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6151ae4dcae5a0ed3e9194c0d994e8d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/6151ae4dcae5a0ed3e9194c0d994e8d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddfb7e8eb34b476cb3a5cc6aeae1b414.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddfb7e8eb34b476cb3a5cc6aeae1b414.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/356742ded4619131733f009e7f44bdb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/356742ded4619131733f009e7f44bdb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d522efc0adefdf878a187d68287ccac7.jpg\" _src=\"http://yanxuan.nosdn.127.net/d522efc0adefdf878a187d68287ccac7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd385aa80f06967d8c120ee2a73ebdea.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd385aa80f06967d8c120ee2a73ebdea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a383ec27f0d0fecf6b218a6434a6537.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a383ec27f0d0fecf6b218a6434a6537.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd76c5d83bdfac3eaef226032e9f2f1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd76c5d83bdfac3eaef226032e9f2f1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f37bf734bedcb5fc34f96a2d3ce21362.jpg\" _src=\"http://yanxuan.nosdn.127.net/f37bf734bedcb5fc34f96a2d3ce21362.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9426b170263b5f2e60b4e349002fb453.jpg\" _src=\"http://yanxuan.nosdn.127.net/9426b170263b5f2e60b4e349002fb453.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02c8fd2d4afb11e4ebfe7e675725f8b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/02c8fd2d4afb11e4ebfe7e675725f8b9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55114d32fb55124afb57fa5f96c7aad6.jpg\" _src=\"http://yanxuan.nosdn.127.net/55114d32fb55124afb57fa5f96c7aad6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c812cb0cf47dfb2b0e0dbdd4e2ae2d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c812cb0cf47dfb2b0e0dbdd4e2ae2d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8491553451f68f13de7d88abd32e80bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/8491553451f68f13de7d88abd32e80bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2358865b0b2916d7b4c85105828e6f5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/2358865b0b2916d7b4c85105828e6f5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d4a761f631987bcb1542cee33c35661.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d4a761f631987bcb1542cee33c35661.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af64442ed12ecc4ec0a8f1053f0e6c4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/af64442ed12ecc4ec0a8f1053f0e6c4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d00f1aa2e519c822a180024983611962.jpg\" _src=\"http://yanxuan.nosdn.127.net/d00f1aa2e519c822a180024983611962.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4dca882b9a0a583456f322030d96d99f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4dca882b9a0a583456f322030d96d99f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a95ed3ffbb239954cc0f1089600847cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/a95ed3ffbb239954cc0f1089600847cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3783189e151670cae90114ac96208749.jpg\" _src=\"http://yanxuan.nosdn.127.net/3783189e151670cae90114ac96208749.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ea89e25888731072a7838f367efe40cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/ea89e25888731072a7838f367efe40cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f3d87a044500179907d61e7984785b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f3d87a044500179907d61e7984785b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfc62369d2cebd727c24356199b3dfc6.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfc62369d2cebd727c24356199b3dfc6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be23add374cfc9344889d449a537159c.jpg\" _src=\"http://yanxuan.nosdn.127.net/be23add374cfc9344889d449a537159c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/113f624f32c22d14b8fe49495d275bce.jpg\" _src=\"http://yanxuan.nosdn.127.net/113f624f32c22d14b8fe49495d275bce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ed060c62699d53a8d04451061aed0a95.jpg\" _src=\"http://yanxuan.nosdn.127.net/ed060c62699d53a8d04451061aed0a95.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a5cc33cd7c28a4c6dbb12e24c5b95e17.jpg\" _src=\"http://yanxuan.nosdn.127.net/a5cc33cd7c28a4c6dbb12e24c5b95e17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ea47a643df6b81539cb50e83585febf.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ea47a643df6b81539cb50e83585febf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37bd564f186c644e582eb5056597fe2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/37bd564f186c644e582eb5056597fe2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b47fe758560f31f84441a5420c2777e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b47fe758560f31f84441a5420c2777e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/079946aa8f0edab416032a761e69c874.jpg\" _src=\"http://yanxuan.nosdn.127.net/079946aa8f0edab416032a761e69c874.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fab6ee083f738fe81e836f5b46345b8c.jpg\" _src=\"http://yanxuan.nosdn.127.net/fab6ee083f738fe81e836f5b46345b8c.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 2,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/afba3e98110e7a36dea74c5bdfe75e41.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ad953e16ad8c33b714e7af941ce8cd56.png",
      "retail_price": 29,
      "sell_volume": 49864,
      "primary_product_id": 1139013,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1138001,
      "category_id": 1008002,
      "goods_sn": "1138001",
      "name": "北欧简约山形纹绣花抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "精细刺绣，舒适立体",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/5737ca831d2cd44a2242eb0992583faf.jpg\" _src=\"http://yanxuan.nosdn.127.net/5737ca831d2cd44a2242eb0992583faf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1160e68bcdeba98d2aada60af18c03c8.jpg\" _src=\"http://yanxuan.nosdn.127.net/1160e68bcdeba98d2aada60af18c03c8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3772cb0d0f4767217726f9af7faa396.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3772cb0d0f4767217726f9af7faa396.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/715a7f19500f5c28d9f73d37ebb1c557.jpg\" _src=\"http://yanxuan.nosdn.127.net/715a7f19500f5c28d9f73d37ebb1c557.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84238cd8ab59b2fe193b825a3e89fd65.jpg\" _src=\"http://yanxuan.nosdn.127.net/84238cd8ab59b2fe193b825a3e89fd65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f4efe768f21095587d8bb4db202b2e23.jpg\" _src=\"http://yanxuan.nosdn.127.net/f4efe768f21095587d8bb4db202b2e23.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbb5a935340a7ff61de6bec5fa3fd985.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbb5a935340a7ff61de6bec5fa3fd985.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b0750c142e857a922d77999a48760cb9.jpg\" _src=\"http://yanxuan.nosdn.127.net/b0750c142e857a922d77999a48760cb9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d742c6ee8b65f2812784e13c2efd04fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/d742c6ee8b65f2812784e13c2efd04fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3aada66e84ec86907ca941fbc5235f12.jpg\" _src=\"http://yanxuan.nosdn.127.net/3aada66e84ec86907ca941fbc5235f12.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb0fd8620c6d6208773667096709ba2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb0fd8620c6d6208773667096709ba2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82b0a7a951c15b41eb5a4bb688dd74dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/82b0a7a951c15b41eb5a4bb688dd74dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/274fea6d222c1da9c687cb73f0f4f993.jpg\" _src=\"http://yanxuan.nosdn.127.net/274fea6d222c1da9c687cb73f0f4f993.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fc87ced2f7b274139bb079a75f7adf91.jpg\" _src=\"http://yanxuan.nosdn.127.net/fc87ced2f7b274139bb079a75f7adf91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a7f98096222daadf9820e1075670173.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a7f98096222daadf9820e1075670173.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/26501a456d9e85980e12efe92120de56.jpg\" _src=\"http://yanxuan.nosdn.127.net/26501a456d9e85980e12efe92120de56.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7a9fbd6be2b2a3c2c83d4edaad2086a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/7a9fbd6be2b2a3c2c83d4edaad2086a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3bf915e824b8b917c893167a99a3773.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3bf915e824b8b917c893167a99a3773.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/211b5a457edcb05d3f3d21ff69c48398.jpg\" _src=\"http://yanxuan.nosdn.127.net/211b5a457edcb05d3f3d21ff69c48398.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc0105d79ff4744f0680cbd2f87a8060.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc0105d79ff4744f0680cbd2f87a8060.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1da6da8c6b7b52f958fdec1dd7769c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1da6da8c6b7b52f958fdec1dd7769c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88ed21fc61da4f79545941fffce1f68c.jpg\" _src=\"http://yanxuan.nosdn.127.net/88ed21fc61da4f79545941fffce1f68c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6eb4abc57dbd46d6dcc38cac3bd32c68.jpg\" _src=\"http://yanxuan.nosdn.127.net/6eb4abc57dbd46d6dcc38cac3bd32c68.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c54b9b585c2e03559865e086f9b45bd.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c54b9b585c2e03559865e086f9b45bd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f88e9af10088b3a0b4669b27ef2fcadb.jpg\" _src=\"http://yanxuan.nosdn.127.net/f88e9af10088b3a0b4669b27ef2fcadb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b249bac9bf3aa94bf4fffb5ac4d1e70.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b249bac9bf3aa94bf4fffb5ac4d1e70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7ded1405eaa6f687eeb9e31b469d5de.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7ded1405eaa6f687eeb9e31b469d5de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d072d1f04f7d94495227cf25b591744.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d072d1f04f7d94495227cf25b591744.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89f67b83d74f2a18b680bb5e6ef0d721.jpg\" _src=\"http://yanxuan.nosdn.127.net/89f67b83d74f2a18b680bb5e6ef0d721.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/236e948413b249b5ea4c1f6f8e835641.jpg\" _src=\"http://yanxuan.nosdn.127.net/236e948413b249b5ea4c1f6f8e835641.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b799d3613b5e3b87d89a608533473df8.jpg\" _src=\"http://yanxuan.nosdn.127.net/b799d3613b5e3b87d89a608533473df8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e6d4af8873253a0b5ae097c15c3628c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/e6d4af8873253a0b5ae097c15c3628c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fc017dc5a790385f6a96b43cf1a5b867.jpg\" _src=\"http://yanxuan.nosdn.127.net/fc017dc5a790385f6a96b43cf1a5b867.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f10cc90e368fad0bd49fafc3b9047b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f10cc90e368fad0bd49fafc3b9047b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/864bf5646ba2ad778f507c224973bca7.jpg\" _src=\"http://yanxuan.nosdn.127.net/864bf5646ba2ad778f507c224973bca7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0443f772258e35af98be389a08fd85b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/0443f772258e35af98be389a08fd85b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/821926b210f311717fdaa0eccb142e37.jpg\" _src=\"http://yanxuan.nosdn.127.net/821926b210f311717fdaa0eccb142e37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/24d0ab5a259a662501e813cf21d752d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/24d0ab5a259a662501e813cf21d752d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b58c263c7e090c68d77e056c9d9afe27.jpg\" _src=\"http://yanxuan.nosdn.127.net/b58c263c7e090c68d77e056c9d9afe27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d50d8b9f53f54ff0c066de7b39b2601c.jpg\" _src=\"http://yanxuan.nosdn.127.net/d50d8b9f53f54ff0c066de7b39b2601c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b382bfe1d8797e845bbcfd9dce361f76.jpg\" _src=\"http://yanxuan.nosdn.127.net/b382bfe1d8797e845bbcfd9dce361f76.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3aecb3e8d261312596727f56b54a0fa2.jpg\" _src=\"http://yanxuan.nosdn.127.net/3aecb3e8d261312596727f56b54a0fa2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c733463829f1fe8fa61998ae7c2ae37b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c733463829f1fe8fa61998ae7c2ae37b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da2850f298b6cf4108e00a06bbc59821.jpg\" _src=\"http://yanxuan.nosdn.127.net/da2850f298b6cf4108e00a06bbc59821.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd0924729a92af064c2108569e9d9463.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd0924729a92af064c2108569e9d9463.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b819438a87396b0e3cc22202fc19caf0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b819438a87396b0e3cc22202fc19caf0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ea853201f8ad389ae3068f3d765aa44.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ea853201f8ad389ae3068f3d765aa44.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ef9093e1959a79178c32d5fc0fbe996.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ef9093e1959a79178c32d5fc0fbe996.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da1d1a9a1e2afe85b640d573085a3d24.jpg\" _src=\"http://yanxuan.nosdn.127.net/da1d1a9a1e2afe85b640d573085a3d24.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce702a9ac92d3666be5d4de2af5e03ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce702a9ac92d3666be5d4de2af5e03ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b43f6da048bbc7206990d9ff972a23ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/b43f6da048bbc7206990d9ff972a23ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22eb869c0f07b55826e1e183dd498f3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/22eb869c0f07b55826e1e183dd498f3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d2c6bf7e29f0e8380ebef90b3bab2294.jpg\" _src=\"http://yanxuan.nosdn.127.net/d2c6bf7e29f0e8380ebef90b3bab2294.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 3,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/1d388fe2012c52f77732aef17b32a058.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/dbc5b25b824c3b3d7ff43b56ca35eee9.png",
      "retail_price": 79,
      "sell_volume": 5508,
      "primary_product_id": 1139049,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147045,
      "category_id": 1008002,
      "goods_sn": "1147045",
      "name": "清新趣粉系列居家地毯 灰黄条纹",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "条纹色块拼接 软糯温馨",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/baa3d2e8841117edfdf0b77ba4b923a3.jpg\" _src=\"http://yanxuan.nosdn.127.net/baa3d2e8841117edfdf0b77ba4b923a3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8c629e309184f5e1e51cdb10193bf993.jpg\" _src=\"http://yanxuan.nosdn.127.net/8c629e309184f5e1e51cdb10193bf993.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e9f6e41af564fd0cc40a123dce69db4.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e9f6e41af564fd0cc40a123dce69db4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61df354d45227bd4d1870a792cc69b65.jpg\" _src=\"http://yanxuan.nosdn.127.net/61df354d45227bd4d1870a792cc69b65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb315d87c9b79db279e8fe1f0a4ff351.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb315d87c9b79db279e8fe1f0a4ff351.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b43def579fe53f8b3d55f3838a5e98dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/b43def579fe53f8b3d55f3838a5e98dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4844c8fcd50ebca556d83c3b79563e30.jpg\" _src=\"http://yanxuan.nosdn.127.net/4844c8fcd50ebca556d83c3b79563e30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8ec64be5f5e18d9c7c3f8031f843928.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8ec64be5f5e18d9c7c3f8031f843928.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76b3c0e01553f16457d2d86c7a4fcfd6.jpg\" _src=\"http://yanxuan.nosdn.127.net/76b3c0e01553f16457d2d86c7a4fcfd6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fef2ca1994a2fdb6a2ed15c6fcd55e71.jpg\" _src=\"http://yanxuan.nosdn.127.net/fef2ca1994a2fdb6a2ed15c6fcd55e71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02cc37f70c3eb52657303293f20d7273.jpg\" _src=\"http://yanxuan.nosdn.127.net/02cc37f70c3eb52657303293f20d7273.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9970f5e3649225e7922cd16e2552f92.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9970f5e3649225e7922cd16e2552f92.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/73be44d027e0869444fabcf8455f7c41.jpg\" _src=\"http://yanxuan.nosdn.127.net/73be44d027e0869444fabcf8455f7c41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b032b74be52d7f848073d847c4ad2e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b032b74be52d7f848073d847c4ad2e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39422d211ff45305b433f52be48ba594.jpg\" _src=\"http://yanxuan.nosdn.127.net/39422d211ff45305b433f52be48ba594.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/253b600c627a913f11621c4b0efabd9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/253b600c627a913f11621c4b0efabd9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0615bcf15f2a5c242cf8ac8b25954e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0615bcf15f2a5c242cf8ac8b25954e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75c6bb3e19f57b854f3f1c81aebb12a5.jpg\" _src=\"http://yanxuan.nosdn.127.net/75c6bb3e19f57b854f3f1c81aebb12a5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0d8903b362c483a6a361e25db45efad4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0d8903b362c483a6a361e25db45efad4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/861fb97fb4debc078419692924514e82.jpg\" _src=\"http://yanxuan.nosdn.127.net/861fb97fb4debc078419692924514e82.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/743398e0811fd6d35b89c8a381596b78.jpg\" _src=\"http://yanxuan.nosdn.127.net/743398e0811fd6d35b89c8a381596b78.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e9e0833fcc2817458548985fc82743a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e9e0833fcc2817458548985fc82743a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6fc6a7297e038f54bdd793fa4d46b7f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/6fc6a7297e038f54bdd793fa4d46b7f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f9d1f2c5711307a84e2ef3a804eb124e.jpg\" _src=\"http://yanxuan.nosdn.127.net/f9d1f2c5711307a84e2ef3a804eb124e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d43ea14ec1e6a520d204fef585bc2ced.jpg\" _src=\"http://yanxuan.nosdn.127.net/d43ea14ec1e6a520d204fef585bc2ced.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca2cab985f7089ad1d6a94d6dd32ff79.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca2cab985f7089ad1d6a94d6dd32ff79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/adaf13c5db73ab4617b6fa0523281cb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/adaf13c5db73ab4617b6fa0523281cb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7adf7694a6b17807ef8d209b762019ac.jpg\" _src=\"http://yanxuan.nosdn.127.net/7adf7694a6b17807ef8d209b762019ac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e240ae9175c7038ba5aea852ba8d79b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e240ae9175c7038ba5aea852ba8d79b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f996a3aedda46c7035c7e62f15de1b12.jpg\" _src=\"http://yanxuan.nosdn.127.net/f996a3aedda46c7035c7e62f15de1b12.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b8d1f9feac00c6f0400cf1398075afe.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b8d1f9feac00c6f0400cf1398075afe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da97979f5eb5ebc72258275a4dc4f811.jpg\" _src=\"http://yanxuan.nosdn.127.net/da97979f5eb5ebc72258275a4dc4f811.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/836c4651e2517b6fec9378f5b402ee52.jpg\" _src=\"http://yanxuan.nosdn.127.net/836c4651e2517b6fec9378f5b402ee52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aabd8aebb5ba1e110e83549fc4731695.jpg\" _src=\"http://yanxuan.nosdn.127.net/aabd8aebb5ba1e110e83549fc4731695.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b9044c606ecc9f38abbf0221e3ebbd4.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b9044c606ecc9f38abbf0221e3ebbd4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f16bc374ca38229922d2045a665e2748.jpg\" _src=\"http://yanxuan.nosdn.127.net/f16bc374ca38229922d2045a665e2748.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71061c570c309fa87cc40be92015ddc2.jpg\" _src=\"http://yanxuan.nosdn.127.net/71061c570c309fa87cc40be92015ddc2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a96dbfd80979f937ea12a3af9320967f.jpg\" _src=\"http://yanxuan.nosdn.127.net/a96dbfd80979f937ea12a3af9320967f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/108f41fb93d0b1b4a126e5a9f1e4c36b.jpg\" _src=\"http://yanxuan.nosdn.127.net/108f41fb93d0b1b4a126e5a9f1e4c36b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/082055188b9b80a9280d87f0da63f071.jpg\" _src=\"http://yanxuan.nosdn.127.net/082055188b9b80a9280d87f0da63f071.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16785ca3b958e7f7285e60d83cb642dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/16785ca3b958e7f7285e60d83cb642dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddddc261de8e4000c8172e2541375167.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddddc261de8e4000c8172e2541375167.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59e2121b4fded2ec47e9b5465fd3e019.jpg\" _src=\"http://yanxuan.nosdn.127.net/59e2121b4fded2ec47e9b5465fd3e019.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/df574a0bb679353a6dc1fb0ddc5f3eb5.jpg\" _src=\"http://yanxuan.nosdn.127.net/df574a0bb679353a6dc1fb0ddc5f3eb5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09ad34f2c245395cf95d6bfe90e178da.jpg\" _src=\"http://yanxuan.nosdn.127.net/09ad34f2c245395cf95d6bfe90e178da.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 28,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/4675b367076adc6817efd2b1f3746534.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/5cda4a0c4c4ff9728d03186bd053c9ca.png",
      "retail_price": 599,
      "sell_volume": 247,
      "primary_product_id": 1148174,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147046,
      "category_id": 1008002,
      "goods_sn": "1147046",
      "name": "清新趣粉系列居家地毯 条纹间粉",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "多色拼接 舒柔静音",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/b3e30fd4547bd74e73f6de777eb64bcd.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3e30fd4547bd74e73f6de777eb64bcd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c224fa76981b3ee07645807d1ad0ab1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/c224fa76981b3ee07645807d1ad0ab1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77835aad8abf7f76f0c7d3a2733aae69.jpg\" _src=\"http://yanxuan.nosdn.127.net/77835aad8abf7f76f0c7d3a2733aae69.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2062742ccf38bdb099123db791cda7a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/2062742ccf38bdb099123db791cda7a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/952b3584258aae0d3e05ef6b62acdce5.jpg\" _src=\"http://yanxuan.nosdn.127.net/952b3584258aae0d3e05ef6b62acdce5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d30e5094f3a9f6649d70680cbf0b3926.jpg\" _src=\"http://yanxuan.nosdn.127.net/d30e5094f3a9f6649d70680cbf0b3926.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b08dc18762700d9bf8cf76fbe25f2a5d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b08dc18762700d9bf8cf76fbe25f2a5d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c86c5e807cde9caeb442c7f38ec0150.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c86c5e807cde9caeb442c7f38ec0150.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6d698add3680c26585135789f6017aac.jpg\" _src=\"http://yanxuan.nosdn.127.net/6d698add3680c26585135789f6017aac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/308bba84a93420ab84dcf137c1ed40cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/308bba84a93420ab84dcf137c1ed40cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d99cfdded9ca4eaf4b8893a02990a66e.jpg\" _src=\"http://yanxuan.nosdn.127.net/d99cfdded9ca4eaf4b8893a02990a66e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3fc5684fa24b379ab34a348305a771d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/3fc5684fa24b379ab34a348305a771d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/539f5536b64206e201ac52a9812685d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/539f5536b64206e201ac52a9812685d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a9cb4fd76ff556c5d3dede50366c94e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a9cb4fd76ff556c5d3dede50366c94e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4198d8a1ac1b9f8dec283041d4fd2995.jpg\" _src=\"http://yanxuan.nosdn.127.net/4198d8a1ac1b9f8dec283041d4fd2995.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/426ea47932152aea6bc507f3e7e45419.jpg\" _src=\"http://yanxuan.nosdn.127.net/426ea47932152aea6bc507f3e7e45419.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39a503db110fd6af417f2a4f8c69e0dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/39a503db110fd6af417f2a4f8c69e0dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33c5cbd2a8b3f6e822411bd1c3ad7a8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/33c5cbd2a8b3f6e822411bd1c3ad7a8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08dc7ac6cf5bd20b14306161ad801f89.jpg\" _src=\"http://yanxuan.nosdn.127.net/08dc7ac6cf5bd20b14306161ad801f89.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd0c4ae24186570c49ecb6ea6bc4d223.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd0c4ae24186570c49ecb6ea6bc4d223.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/46eaed18b282b3177df608f9e410cfac.jpg\" _src=\"http://yanxuan.nosdn.127.net/46eaed18b282b3177df608f9e410cfac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2e4a411c483653141471eec5c9c9f6fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/2e4a411c483653141471eec5c9c9f6fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e013bfa3e6a997fcce4e526efa5d68fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/e013bfa3e6a997fcce4e526efa5d68fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50bc2637bd5ea29d1d787df548e494c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/50bc2637bd5ea29d1d787df548e494c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ef7aebd62895db555aec269d55cbe14a.jpg\" _src=\"http://yanxuan.nosdn.127.net/ef7aebd62895db555aec269d55cbe14a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb53d78a085c29a0c12ec4c608db20a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb53d78a085c29a0c12ec4c608db20a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b887ad166e42363fe84e7a7a74971b88.jpg\" _src=\"http://yanxuan.nosdn.127.net/b887ad166e42363fe84e7a7a74971b88.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e57ab2325bfacc46a536d2e9f774814b.jpg\" _src=\"http://yanxuan.nosdn.127.net/e57ab2325bfacc46a536d2e9f774814b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2bf04434da86c3ef8f46e034164836a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/2bf04434da86c3ef8f46e034164836a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfa1f11efc7d868ae038fadc5f55096b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfa1f11efc7d868ae038fadc5f55096b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0dd4b31cc78d7f9047948b224221b643.jpg\" _src=\"http://yanxuan.nosdn.127.net/0dd4b31cc78d7f9047948b224221b643.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39a3bc4e36427106682402c687addb1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/39a3bc4e36427106682402c687addb1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae019d3a06a02983f26de10b3b415830.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae019d3a06a02983f26de10b3b415830.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8fef320814c866e80295655a8bcbd81.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8fef320814c866e80295655a8bcbd81.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/980c7827076572b35c5c4c7bb2e65108.jpg\" _src=\"http://yanxuan.nosdn.127.net/980c7827076572b35c5c4c7bb2e65108.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65f907cc355fe1701f3e2822bf631d55.jpg\" _src=\"http://yanxuan.nosdn.127.net/65f907cc355fe1701f3e2822bf631d55.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d27625f9111c8fd1bf19bc428b87a6d2.jpg\" _src=\"http://yanxuan.nosdn.127.net/d27625f9111c8fd1bf19bc428b87a6d2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/714ea85d22a65a2a7698a20ac9cb3320.jpg\" _src=\"http://yanxuan.nosdn.127.net/714ea85d22a65a2a7698a20ac9cb3320.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8ee12c729cf07679d4135ac314c1b37.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8ee12c729cf07679d4135ac314c1b37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0bcb12fdd8d835705ee9ac88b764b441.jpg\" _src=\"http://yanxuan.nosdn.127.net/0bcb12fdd8d835705ee9ac88b764b441.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79124540860c5a26842803b62b46fc8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/79124540860c5a26842803b62b46fc8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca54c7438b6cfe4c139f9a07e9c0b055.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca54c7438b6cfe4c139f9a07e9c0b055.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a4eede58b9d7b516b708bd1bfb18e9df.jpg\" _src=\"http://yanxuan.nosdn.127.net/a4eede58b9d7b516b708bd1bfb18e9df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25db36db73d7b38380b3c829a12770d3.jpg\" _src=\"http://yanxuan.nosdn.127.net/25db36db73d7b38380b3c829a12770d3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c86f1f43a2cc6f25c0d162601fa143b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/c86f1f43a2cc6f25c0d162601fa143b9.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 26,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a4ec154d8a8496dd4aa490c8ec6f8bfd.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/655d718df8107f8e7fd1dc6140e29039.png",
      "retail_price": 599,
      "sell_volume": 225,
      "primary_product_id": 1148175,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147047,
      "category_id": 1008002,
      "goods_sn": "1147047",
      "name": "简约知性系列居家地毯 蓝粉拼接",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "三角几何拼接 超细绒感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/e56e30a2c6cbdeadb1a2b6d00f2e877f.jpg\" _src=\"http://yanxuan.nosdn.127.net/e56e30a2c6cbdeadb1a2b6d00f2e877f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d14496c74886e92b3a3f30692756e77a.jpg\" _src=\"http://yanxuan.nosdn.127.net/d14496c74886e92b3a3f30692756e77a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0a371e340849de0ca0c628021cbc0014.jpg\" _src=\"http://yanxuan.nosdn.127.net/0a371e340849de0ca0c628021cbc0014.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a5a80c783e941991414cd8ede724312.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a5a80c783e941991414cd8ede724312.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37a49c90311b2661a24887ff2de448c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/37a49c90311b2661a24887ff2de448c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e25787020a28bbb6e9f2a220aa2dd442.jpg\" _src=\"http://yanxuan.nosdn.127.net/e25787020a28bbb6e9f2a220aa2dd442.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52b8beb545c2ae0115522908ac352a39.jpg\" _src=\"http://yanxuan.nosdn.127.net/52b8beb545c2ae0115522908ac352a39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afaa8978308f2531ada6aaaf63c56347.jpg\" _src=\"http://yanxuan.nosdn.127.net/afaa8978308f2531ada6aaaf63c56347.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18789d3aacac9d2de6a6b21cfb7aec53.jpg\" _src=\"http://yanxuan.nosdn.127.net/18789d3aacac9d2de6a6b21cfb7aec53.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/154e9f3504ada7cdadcb906ee01450c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/154e9f3504ada7cdadcb906ee01450c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3326e16fbfee855392404e970bd5aa4c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3326e16fbfee855392404e970bd5aa4c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b5b0d22fc526776cef8e756dff60dd1.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b5b0d22fc526776cef8e756dff60dd1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48dd357aa1abc60c01b3fbf8dacb2694.jpg\" _src=\"http://yanxuan.nosdn.127.net/48dd357aa1abc60c01b3fbf8dacb2694.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27e574eab03093d302f01e5ceb42d0af.jpg\" _src=\"http://yanxuan.nosdn.127.net/27e574eab03093d302f01e5ceb42d0af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/30228bd984383c97633eef50ca556406.jpg\" _src=\"http://yanxuan.nosdn.127.net/30228bd984383c97633eef50ca556406.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/baa3cc805dc0afb4257c30466771535a.jpg\" _src=\"http://yanxuan.nosdn.127.net/baa3cc805dc0afb4257c30466771535a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/daa37937c3440919e597e4954e68f646.jpg\" _src=\"http://yanxuan.nosdn.127.net/daa37937c3440919e597e4954e68f646.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82df87910187f081e2a4d5f5a06df4cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/82df87910187f081e2a4d5f5a06df4cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eaa197c3d63c8479e38f46595df50a5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/eaa197c3d63c8479e38f46595df50a5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/56cf9f1b8de8627ad0d064843d97cd96.jpg\" _src=\"http://yanxuan.nosdn.127.net/56cf9f1b8de8627ad0d064843d97cd96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99ad88418c88c550b183dc12a9280a1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/99ad88418c88c550b183dc12a9280a1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a84aafb6ddbe25f32bddc4f843ad35d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/a84aafb6ddbe25f32bddc4f843ad35d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ce402bfb9d08603259264e9115166b2.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ce402bfb9d08603259264e9115166b2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a7248d14d630770dfff1b17350219ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a7248d14d630770dfff1b17350219ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/43113bc52b7eece12f777092d9b04c3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/43113bc52b7eece12f777092d9b04c3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbe65886e9405ceb1a43fb3097fd709a.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbe65886e9405ceb1a43fb3097fd709a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e098163e428171418a77c077a8330299.jpg\" _src=\"http://yanxuan.nosdn.127.net/e098163e428171418a77c077a8330299.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbb9a88692c9621652244844bf0b299d.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbb9a88692c9621652244844bf0b299d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d8264c945ccb68d432dcaeb86e3e4ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d8264c945ccb68d432dcaeb86e3e4ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e0a467456d69bc746e6bd7797f6963b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e0a467456d69bc746e6bd7797f6963b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a58d0c630b0e2f51fa49aef8687a9e16.jpg\" _src=\"http://yanxuan.nosdn.127.net/a58d0c630b0e2f51fa49aef8687a9e16.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1de7c562962e54da6a63e749634eb008.jpg\" _src=\"http://yanxuan.nosdn.127.net/1de7c562962e54da6a63e749634eb008.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8931ee6e2b4b3ed3454184093b6471ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/8931ee6e2b4b3ed3454184093b6471ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b032ca9815193ec258be3ffa0a25da3.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b032ca9815193ec258be3ffa0a25da3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfd12f882162e93008c97bff3187f694.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfd12f882162e93008c97bff3187f694.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79d69e15728310ec458ec665a287fc87.jpg\" _src=\"http://yanxuan.nosdn.127.net/79d69e15728310ec458ec665a287fc87.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e10b0c8d89689483eceea36aa330deb4.jpg\" _src=\"http://yanxuan.nosdn.127.net/e10b0c8d89689483eceea36aa330deb4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88c5b10b0916839ae7cf6ca1b8c8d83f.jpg\" _src=\"http://yanxuan.nosdn.127.net/88c5b10b0916839ae7cf6ca1b8c8d83f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/17b3ace86142f2b8c7f29ed10d1dba55.jpg\" _src=\"http://yanxuan.nosdn.127.net/17b3ace86142f2b8c7f29ed10d1dba55.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83f9993c4dda4898693ba3fe9f313c1f.jpg\" _src=\"http://yanxuan.nosdn.127.net/83f9993c4dda4898693ba3fe9f313c1f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9310f4e403eb5db6107bfc280c3e6cf8.jpg\" _src=\"http://yanxuan.nosdn.127.net/9310f4e403eb5db6107bfc280c3e6cf8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ba895b4d7507984a26344d7c03db550.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ba895b4d7507984a26344d7c03db550.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/34f3faaad28a93f140f3f1b78def4bce.jpg\" _src=\"http://yanxuan.nosdn.127.net/34f3faaad28a93f140f3f1b78def4bce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/355dc9d6e4a8a1a8561183641ef2890a.jpg\" _src=\"http://yanxuan.nosdn.127.net/355dc9d6e4a8a1a8561183641ef2890a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2b6a2155e30bf99750756ec4fb99f11.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2b6a2155e30bf99750756ec4fb99f11.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 29,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/6f162e1b98906c2a02c75b40ff9659d3.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/bda805b0a2464b6ec33c18981565e50e.png",
      "retail_price": 559,
      "sell_volume": 199,
      "primary_product_id": 1148176,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147048,
      "category_id": 1008002,
      "goods_sn": "1147048",
      "name": "简约知性系列居家地毯 蓝灰格",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "沉稳双拼色 居家温柔伴护",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/037e5909a5bec975c67bf61d193d7b72.jpg\" _src=\"http://yanxuan.nosdn.127.net/037e5909a5bec975c67bf61d193d7b72.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88486bfa3d7bd68c7780df5cc01e7a7d.jpg\" _src=\"http://yanxuan.nosdn.127.net/88486bfa3d7bd68c7780df5cc01e7a7d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77c2d1819d99dde7cad8c140048a46aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/77c2d1819d99dde7cad8c140048a46aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f49aed0ebcd5c54f3edb8240921e3a46.jpg\" _src=\"http://yanxuan.nosdn.127.net/f49aed0ebcd5c54f3edb8240921e3a46.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60b923642f98ca62ca3d9a6fe0db8800.jpg\" _src=\"http://yanxuan.nosdn.127.net/60b923642f98ca62ca3d9a6fe0db8800.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/782d6edfc30d1a53711d5f0f6145f8fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/782d6edfc30d1a53711d5f0f6145f8fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b10a5a5f29340056cb6b1673420f46c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b10a5a5f29340056cb6b1673420f46c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2e721a8f26030ba31f0b290c47ba232.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2e721a8f26030ba31f0b290c47ba232.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77d18b39a7d8b603b869ca4cb8d7235b.jpg\" _src=\"http://yanxuan.nosdn.127.net/77d18b39a7d8b603b869ca4cb8d7235b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c266d8f75bc074531033430882a93d8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/c266d8f75bc074531033430882a93d8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ceb7a59b3c56f7ced051cae61d70daf6.jpg\" _src=\"http://yanxuan.nosdn.127.net/ceb7a59b3c56f7ced051cae61d70daf6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0db841700c868c08d627f01c354b013c.jpg\" _src=\"http://yanxuan.nosdn.127.net/0db841700c868c08d627f01c354b013c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/008ea04b11a0f68116e5eb180ca8a6a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/008ea04b11a0f68116e5eb180ca8a6a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfa3513280704216372dade1751b2bc6.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfa3513280704216372dade1751b2bc6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1287987157d7a1767ccaec835bb82b17.jpg\" _src=\"http://yanxuan.nosdn.127.net/1287987157d7a1767ccaec835bb82b17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/041f4c058fd201716c456d32588e0611.jpg\" _src=\"http://yanxuan.nosdn.127.net/041f4c058fd201716c456d32588e0611.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22832d570b7eaf8153d5038d9095b990.jpg\" _src=\"http://yanxuan.nosdn.127.net/22832d570b7eaf8153d5038d9095b990.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5651dedb8b4d5c1d40345f13a4ad622.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5651dedb8b4d5c1d40345f13a4ad622.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b988f3146c079e488eeb05ba03cae37.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b988f3146c079e488eeb05ba03cae37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6d53d4374b9a800da1eb215b6215b403.jpg\" _src=\"http://yanxuan.nosdn.127.net/6d53d4374b9a800da1eb215b6215b403.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1abd7dd665582e0eb1c8e4bd6196b6cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1abd7dd665582e0eb1c8e4bd6196b6cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39561bb5901a7a80bf362bf4b7b96d30.jpg\" _src=\"http://yanxuan.nosdn.127.net/39561bb5901a7a80bf362bf4b7b96d30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99eff53c1440f72152c2b264c22244a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/99eff53c1440f72152c2b264c22244a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e54bd5c82506db1eed358edcdbd6ef8.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e54bd5c82506db1eed358edcdbd6ef8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83ca52b41e1907932bc55330fd5a5cad.jpg\" _src=\"http://yanxuan.nosdn.127.net/83ca52b41e1907932bc55330fd5a5cad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f58dc91de46bbf93fbf054de64958aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f58dc91de46bbf93fbf054de64958aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08d20c7dc0ae462a176ac52a58e7b297.jpg\" _src=\"http://yanxuan.nosdn.127.net/08d20c7dc0ae462a176ac52a58e7b297.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca1db2649c0a5c67ed319cb212332380.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca1db2649c0a5c67ed319cb212332380.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2feac4d0a9ef0053863b81e37f7fe9fe.jpg\" _src=\"http://yanxuan.nosdn.127.net/2feac4d0a9ef0053863b81e37f7fe9fe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9d2fa42d4fec3abd1c151a8dbdab0ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9d2fa42d4fec3abd1c151a8dbdab0ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e78a8555da079fb963f78fc9149f93cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/e78a8555da079fb963f78fc9149f93cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5384e883e1e96640d1adfca1c2e511f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5384e883e1e96640d1adfca1c2e511f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c8ec5307f7f0c5a3dcea9916bbbf091.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c8ec5307f7f0c5a3dcea9916bbbf091.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c59d89c8b46e0e740fd6d8f40071422.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c59d89c8b46e0e740fd6d8f40071422.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f5640cac8b41175cf3fb620f25ed7ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f5640cac8b41175cf3fb620f25ed7ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20ab37f417610381659ad47de48aa42f.jpg\" _src=\"http://yanxuan.nosdn.127.net/20ab37f417610381659ad47de48aa42f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f676f5243a835cb63d76e20423666337.jpg\" _src=\"http://yanxuan.nosdn.127.net/f676f5243a835cb63d76e20423666337.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b9e1a348d1766c803f9b31221f94553.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b9e1a348d1766c803f9b31221f94553.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a49199ab0ee762df58a2dce4bd26b1e3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a49199ab0ee762df58a2dce4bd26b1e3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4635e2b0daeca9d6dbaf66dc6a74b2f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/4635e2b0daeca9d6dbaf66dc6a74b2f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2d05ee8ffcca5df74090153c8892cb4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/2d05ee8ffcca5df74090153c8892cb4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60c532e803c2d4a75c3da1200797d29c.jpg\" _src=\"http://yanxuan.nosdn.127.net/60c532e803c2d4a75c3da1200797d29c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75b9feace19e5c3c2e5a9e8dca01a0f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/75b9feace19e5c3c2e5a9e8dca01a0f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f5ef8ad3f27f9f6dd1826afe0494c29.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f5ef8ad3f27f9f6dd1826afe0494c29.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50aab2e77e905e1f0c1a71ec25739207.jpg\" _src=\"http://yanxuan.nosdn.127.net/50aab2e77e905e1f0c1a71ec25739207.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 30,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/3386744ee6833d13a6f6b843cb35f6c6.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/fd7920a2eadd10fa10c0c03959a2abe0.png",
      "retail_price": 559,
      "sell_volume": 183,
      "primary_product_id": 1148177,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    }
  ],
  "currentNav": {
    "id": 1008002,
    "name": "布艺软装",
    "keywords": "",
    "front_desc": "换个软装，换个家",
    "parent_id": 1005000,
    "sort_order": 6,
    "show_index": 4,
    "is_show": 1,
    "banner_url": "http://yanxuan.nosdn.127.net/8bbcd7de60a678846664af998f57e71c.png",
    "icon_url": "",
    "img_url": "",
    "wap_banner_url": "http://yanxuan.nosdn.127.net/2e2fb4f2856a021bbcd1b4c8400f2b06.png",
    "level": "L2",
    "type": 0,
    "front_name": "各种风格软装装点你的家"
  }
}
```

### 获取商品详情数据

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/goods/detailaction `

**请求方式：**

- GET 

**参数：** 

| 参数名    | 必选  | 类型     | 说明             |
|:------ |:--- |:------ | -------------- |
| id     | 是   | int    | 商品列表或搜索结果里的id号 |
| openId | 是   | string | 无              |

**返回示例**

```json
{
  "info": {
    "id": 1009024,
    "category_id": 1008002,
    "goods_sn": "1009024",
    "name": "日式和风懒人沙发",
    "brand_id": 0,
    "goods_number": 100,
    "keywords": "",
    "goods_brief": "优质莱卡纯棉，和风家居新体验",
    "goods_desc": "<p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/34a6a0daa3f7a397a38aad14cb9e90fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/34a6a0daa3f7a397a38aad14cb9e90fa.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/76637af0eec246b318cb129b768de637.jpg\" _src=\"http://yanxuan.nosdn.127.net/76637af0eec246b318cb129b768de637.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18fee22626e61fc1d1a01916914016ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/18fee22626e61fc1d1a01916914016ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91f57a9bb142e1c1e2ff0bbea6f9af96.jpg\" _src=\"http://yanxuan.nosdn.127.net/91f57a9bb142e1c1e2ff0bbea6f9af96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/252d80fd75eb1254d746d0b57c267650.jpg\" _src=\"http://yanxuan.nosdn.127.net/252d80fd75eb1254d746d0b57c267650.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b07697992a2b14de6fd0a5811936d71.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b07697992a2b14de6fd0a5811936d71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c499439d6081bb4e836955b7514c1b96.jpg\" _src=\"http://yanxuan.nosdn.127.net/c499439d6081bb4e836955b7514c1b96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bed437fdc091d020a8f805bcc8830bd8.jpg\" _src=\"http://yanxuan.nosdn.127.net/bed437fdc091d020a8f805bcc8830bd8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fc5febdb817abd7a1040bab03f048b7.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fc5febdb817abd7a1040bab03f048b7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a0417b3986c9dc082124fcc360390021.jpg\" _src=\"http://yanxuan.nosdn.127.net/a0417b3986c9dc082124fcc360390021.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a5c9d24c652d4dee7946ef925105f3f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/a5c9d24c652d4dee7946ef925105f3f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b10272c58f95dd6737ce1cd41452a21d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b10272c58f95dd6737ce1cd41452a21d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/510c6ef36760238b38ed59cd6e47a21f.png\" _src=\"http://yanxuan.nosdn.127.net/510c6ef36760238b38ed59cd6e47a21f.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6371348b917c021c55dc393fc59d4d28.png\" _src=\"http://yanxuan.nosdn.127.net/6371348b917c021c55dc393fc59d4d28.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de4079b128e57c5c0fa8a8177e9bc6e7.png\" _src=\"http://yanxuan.nosdn.127.net/de4079b128e57c5c0fa8a8177e9bc6e7.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/160966fbc772787f824dc1dbd5afb16d.png\" _src=\"http://yanxuan.nosdn.127.net/160966fbc772787f824dc1dbd5afb16d.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb3c8d3f10f2aca0908871c8e598aa0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb3c8d3f10f2aca0908871c8e598aa0e.jpg\"/></p><p><br/></p>",
    "is_on_sale": 1,
    "add_time": 0,
    "sort_order": 1,
    "is_delete": 0,
    "attribute_category": 0,
    "counter_price": 0,
    "extra_price": 0,
    "is_new": 0,
    "goods_unit": "件",
    "primary_pic_url": "http://yanxuan.nosdn.127.net/bcaf7ee314af7dbfb04612087e563249.jpg",
    "list_pic_url": "http://yanxuan.nosdn.127.net/149dfa87a7324e184c5526ead81de9ad.png",
    "retail_price": 599,
    "sell_volume": 2918,
    "primary_product_id": 1008052,
    "unit_price": 0,
    "promotion_desc": "限时购",
    "promotion_tag": "",
    "app_exclusive_price": 0,
    "is_app_exclusive": 0,
    "is_limited": 0,
    "is_hot": 0
  },
  "gallery": [
    {
      "id": 33,
      "goods_id": 1009024,
      "img_url": "http://yanxuan.nosdn.127.net/9460f6b30661548c4a864607bfcdf4ca.jpg",
      "img_desc": "",
      "sort_order": 5
    },
    {
      "id": 34,
      "goods_id": 1009024,
      "img_url": "http://yanxuan.nosdn.127.net/acbdb480bcad193fad77ef6c4f52192e.jpg",
      "img_desc": "",
      "sort_order": 5
    },
    {
      "id": 35,
      "goods_id": 1009024,
      "img_url": "http://yanxuan.nosdn.127.net/e6feb5f4a0989d212bce068d4907657d.jpg",
      "img_desc": "",
      "sort_order": 5
    },
    {
      "id": 36,
      "goods_id": 1009024,
      "img_url": "http://yanxuan.nosdn.127.net/6059ab6e106d97c29d5723c1d6f1a11f.jpg",
      "img_desc": "",
      "sort_order": 5
    }
  ],
  "attribute": [
    {
      "value": "65*65*43cm",
      "name": "规格"
    },
    {
      "value": "外套帆布：100%棉；外套弹力布：锦纶80%氨纶20%",
      "name": "外套材质"
    },
    {
      "value": "内胆面料：100%锦纶；填充物：聚苯乙烯（发泡粒子）",
      "name": "内胆材质"
    },
    {
      "value": "本品为人工填充粒子，重量难免会有误差，敬请谅解。同时产品在运输过程中受挤压，也可能会造成凹陷。储存时请避免重物挤压以引起泡沫粒子塌陷。",
      "name": "*温馨提示"
    }
  ],
  "issue": [
    {
      "id": 1,
      "goods_id": "1127052",
      "question": "购买运费如何收取？",
      "answer": "单笔订单金额（不含运费）满88元免邮费；不满88元，每单收取10元运费。\n(港澳台地区需满"
    },
    {
      "id": 2,
      "goods_id": "1127052",
      "question": "使用什么快递发货？",
      "answer": "严选默认使用顺丰快递发货（个别商品使用其他快递），配送范围覆盖全国大部分地区（港澳台地区除"
    },
    {
      "id": 3,
      "goods_id": "1127052",
      "question": "如何申请退货？",
      "answer": "1.自收到商品之日起30日内，顾客可申请无忧退货，退款将原路返还，不同的银行处理时间不同，"
    },
    {
      "id": 4,
      "goods_id": "1127052",
      "question": "如何开具发票？",
      "answer": "1.如需开具普通发票，请在下单时选择“我要开发票”并填写相关信息（APP仅限2.4.0及以"
    }
  ],
  "comment": {
    "count": 30,
    "data": {
      "content": "好舒服！可以变换各种形状！比我之前在朋友家看到的懒人沙发好很多啊！",
      "nickname": "heyushuo",
      "avatar": "http://img1.imgtn.bdimg.com/it/u=1514241375,2114605636&fm=27&gp=0.jpg",
      "pic_list": [
        {
          "id": 289,
          "comment_id": 241,
          "pic_url": "https://yanxuan.nosdn.127.net/a3bd6f130fe3ee340037a37b6c721d16.jpg",
          "sort_order": 5
        }
      ]
    }
  },
  "brand": [],
  "productList": [
    {
      "id": 1009024,
      "category_id": 1008002,
      "goods_sn": "1009024",
      "name": "日式和风懒人沙发",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "优质莱卡纯棉，和风家居新体验",
      "goods_desc": "<p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/34a6a0daa3f7a397a38aad14cb9e90fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/34a6a0daa3f7a397a38aad14cb9e90fa.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/76637af0eec246b318cb129b768de637.jpg\" _src=\"http://yanxuan.nosdn.127.net/76637af0eec246b318cb129b768de637.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18fee22626e61fc1d1a01916914016ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/18fee22626e61fc1d1a01916914016ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91f57a9bb142e1c1e2ff0bbea6f9af96.jpg\" _src=\"http://yanxuan.nosdn.127.net/91f57a9bb142e1c1e2ff0bbea6f9af96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/252d80fd75eb1254d746d0b57c267650.jpg\" _src=\"http://yanxuan.nosdn.127.net/252d80fd75eb1254d746d0b57c267650.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b07697992a2b14de6fd0a5811936d71.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b07697992a2b14de6fd0a5811936d71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c499439d6081bb4e836955b7514c1b96.jpg\" _src=\"http://yanxuan.nosdn.127.net/c499439d6081bb4e836955b7514c1b96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bed437fdc091d020a8f805bcc8830bd8.jpg\" _src=\"http://yanxuan.nosdn.127.net/bed437fdc091d020a8f805bcc8830bd8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fc5febdb817abd7a1040bab03f048b7.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fc5febdb817abd7a1040bab03f048b7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a0417b3986c9dc082124fcc360390021.jpg\" _src=\"http://yanxuan.nosdn.127.net/a0417b3986c9dc082124fcc360390021.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a5c9d24c652d4dee7946ef925105f3f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/a5c9d24c652d4dee7946ef925105f3f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b10272c58f95dd6737ce1cd41452a21d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b10272c58f95dd6737ce1cd41452a21d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/510c6ef36760238b38ed59cd6e47a21f.png\" _src=\"http://yanxuan.nosdn.127.net/510c6ef36760238b38ed59cd6e47a21f.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6371348b917c021c55dc393fc59d4d28.png\" _src=\"http://yanxuan.nosdn.127.net/6371348b917c021c55dc393fc59d4d28.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de4079b128e57c5c0fa8a8177e9bc6e7.png\" _src=\"http://yanxuan.nosdn.127.net/de4079b128e57c5c0fa8a8177e9bc6e7.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/160966fbc772787f824dc1dbd5afb16d.png\" _src=\"http://yanxuan.nosdn.127.net/160966fbc772787f824dc1dbd5afb16d.png\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb3c8d3f10f2aca0908871c8e598aa0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb3c8d3f10f2aca0908871c8e598aa0e.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 1,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/bcaf7ee314af7dbfb04612087e563249.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/149dfa87a7324e184c5526ead81de9ad.png",
      "retail_price": 599,
      "sell_volume": 2918,
      "primary_product_id": 1008052,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1015007,
      "category_id": 1008002,
      "goods_sn": "1015007",
      "name": "典雅美式全棉刺绣抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "典雅毛线绣，精致工艺",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/66640f55aeb668ac9df6e26b6b30adb5.jpg\" _src=\"http://yanxuan.nosdn.127.net/66640f55aeb668ac9df6e26b6b30adb5.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/42852faba5623c6dc5be451d80e5df03.jpg\" _src=\"http://yanxuan.nosdn.127.net/42852faba5623c6dc5be451d80e5df03.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48ce93c6f6a731778c505442f163b09e.jpg\" _src=\"http://yanxuan.nosdn.127.net/48ce93c6f6a731778c505442f163b09e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02a3abee9bb3e22f27781ced8774d1ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/02a3abee9bb3e22f27781ced8774d1ab.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c62a27145e1045879e3f2b97b9f86b4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/c62a27145e1045879e3f2b97b9f86b4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48baaafe4ea4c32242c57e58ce8e139f.jpg\" _src=\"http://yanxuan.nosdn.127.net/48baaafe4ea4c32242c57e58ce8e139f.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99549f0375b108240866a09a0a2527d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/99549f0375b108240866a09a0a2527d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/341529ba80d91c5304680be8f524a626.jpg\" _src=\"http://yanxuan.nosdn.127.net/341529ba80d91c5304680be8f524a626.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b15e35e9d8c04288dfb7546b1f743c17.jpg\" _src=\"http://yanxuan.nosdn.127.net/b15e35e9d8c04288dfb7546b1f743c17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c0ebf7949133cb382b6bf18c8a5a1c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c0ebf7949133cb382b6bf18c8a5a1c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfd25d0fa6dc13a335877360e3dab8d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfd25d0fa6dc13a335877360e3dab8d1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbcc420cef18e4a43589198ebfcc4fd1.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbcc420cef18e4a43589198ebfcc4fd1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15aa3e3ed45714d29ca062499db930ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/15aa3e3ed45714d29ca062499db930ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab6963b4e529810577f3e428c9d10af6.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab6963b4e529810577f3e428c9d10af6.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 4,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/d16d6fb25f3d6d8c356fcd8e178bdd26.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/a2045004de8a6225289376ad54317fc8.png",
      "retail_price": 59,
      "sell_volume": 133,
      "primary_product_id": 1013024,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1020000,
      "category_id": 1008002,
      "goods_sn": "1020000",
      "name": "升级款记忆绵护椎腰靠",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "人体工学设计，缓解腰背疼痛",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/8176934e414ec6c85078cb64322fe336.jpg\" _src=\"http://yanxuan.nosdn.127.net/8176934e414ec6c85078cb64322fe336.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33ff256b2f69de517f567ebb993dd08e.jpg\" _src=\"http://yanxuan.nosdn.127.net/33ff256b2f69de517f567ebb993dd08e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5204e4f7c7fa00866e270a93ec85a596.jpg\" _src=\"http://yanxuan.nosdn.127.net/5204e4f7c7fa00866e270a93ec85a596.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f3aed0164b92344f17ffbc0b8fc7ade.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f3aed0164b92344f17ffbc0b8fc7ade.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d2d94d8f0f10f17183954b69d09e2bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d2d94d8f0f10f17183954b69d09e2bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3921600dd00e2c49a7414035111b767d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3921600dd00e2c49a7414035111b767d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aef3c726fec0be6ce17089e06e753d4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/aef3c726fec0be6ce17089e06e753d4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/446fbad756b6327898cee40e7b67a0b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/446fbad756b6327898cee40e7b67a0b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0950b4fa1cac49eece29af35c6e69e4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/0950b4fa1cac49eece29af35c6e69e4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf7e88b2b57641ab81bbf36351db5ff8.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf7e88b2b57641ab81bbf36351db5ff8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d66b4714682aaff4ab082980a44b46.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d66b4714682aaff4ab082980a44b46.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7f2d82d7a5622dd9f6b0d44faed9fda.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7f2d82d7a5622dd9f6b0d44faed9fda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7fdc566d101b7cf73cee32f55b0f945.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7fdc566d101b7cf73cee32f55b0f945.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e04202364d1a0a1dc1a2a1ea871e45e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e04202364d1a0a1dc1a2a1ea871e45e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b3135ad6c01a2675fc7e96f6643ff7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b3135ad6c01a2675fc7e96f6643ff7f.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 15,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/84563d90b0c10c4d4a8229fd34cb4063.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/819fdf1f635a694166bcfdd426416e8c.png",
      "retail_price": 79,
      "sell_volume": 8586,
      "primary_product_id": 1018000,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1030001,
      "category_id": 1008002,
      "goods_sn": "1030001",
      "name": "160*230羊毛手工地毯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "印度进口，手工编织，简约百搭",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/fbe953060dd4282539ee78e22f9c326c.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbe953060dd4282539ee78e22f9c326c.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb6320b1b19fe349fca98dcb509ccb41.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb6320b1b19fe349fca98dcb509ccb41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e3517025dc8da160277d7c80c55a83f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e3517025dc8da160277d7c80c55a83f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c6d902b098a5009871e7dd2fc47d4aae.jpg\" _src=\"http://yanxuan.nosdn.127.net/c6d902b098a5009871e7dd2fc47d4aae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15b721ac1796a6a93c2925c45fbafa91.jpg\" _src=\"http://yanxuan.nosdn.127.net/15b721ac1796a6a93c2925c45fbafa91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c1e30ecc74b5b25869f892f51d4472b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c1e30ecc74b5b25869f892f51d4472b0.jpg\" style=\"\"/></p><p><br/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7ddc57f40d4ec7d7e1069fc24438e93.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7ddc57f40d4ec7d7e1069fc24438e93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/68e501bd5f6f2018ee275af62edcebce.jpg\" _src=\"http://yanxuan.nosdn.127.net/68e501bd5f6f2018ee275af62edcebce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6cd10a4cc89e2067421632172382410c.jpg\" _src=\"http://yanxuan.nosdn.127.net/6cd10a4cc89e2067421632172382410c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/81d9b02cc74f846bb29bfc57b4d8dab1.jpg\" _src=\"http://yanxuan.nosdn.127.net/81d9b02cc74f846bb29bfc57b4d8dab1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/30a9e77d7e0cab9b389bc4a7f4a0be13.jpg\" _src=\"http://yanxuan.nosdn.127.net/30a9e77d7e0cab9b389bc4a7f4a0be13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50513c57074971334c4b715d8b3cdfa1.jpg\" _src=\"http://yanxuan.nosdn.127.net/50513c57074971334c4b715d8b3cdfa1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5497b96a17e01db88d3b8999d78e111d.jpg\" _src=\"http://yanxuan.nosdn.127.net/5497b96a17e01db88d3b8999d78e111d.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3311094b3f6ac170477dbf31fdc36a43.jpg\" _src=\"http://yanxuan.nosdn.127.net/3311094b3f6ac170477dbf31fdc36a43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb7a1c7b6c6989af9c42a4e66de098e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb7a1c7b6c6989af9c42a4e66de098e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ac42cbdfaa06c00a1bbd22fd63308546.jpg\" _src=\"http://yanxuan.nosdn.127.net/ac42cbdfaa06c00a1bbd22fd63308546.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0d2bf9139a0ca351f0ae4cabece86277.jpg\" _src=\"http://yanxuan.nosdn.127.net/0d2bf9139a0ca351f0ae4cabece86277.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da1c0eef412d5ff9761a8659fa64d91b.jpg\" _src=\"http://yanxuan.nosdn.127.net/da1c0eef412d5ff9761a8659fa64d91b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba7017652cf73419da57393bb02ca6de.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba7017652cf73419da57393bb02ca6de.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 25,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/ca0d9199db70d7b7f2b9b2ea673c74a4.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/88dc5d80c6f84102f003ecd69c86e1cf.png",
      "retail_price": 969,
      "sell_volume": 657,
      "primary_product_id": 1029001,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1030002,
      "category_id": 1008002,
      "goods_sn": "1030002",
      "name": "160*230羊毛圈绒枪刺地毯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "印度进口，手工枪刺，简约百搭",
      "goods_desc": "<p><video id=\"tmpVedio0\" class=\"edui-upload-video video-js vjs-default-skin video-js\" controls=\"\" preload=\"auto\" width=\"100%\" height=\"\" data-setup=\"{}\"><source src=\"http://yanxuan.nosdn.127.net/4ca24b2fa0043eb7435d1ca24312b689.mp4\" type=\"video/mp4\"/></video>‍</p><p><img src=\"http://yanxuan.nosdn.127.net/4c409ac170dafe286e2cbd918b30a388.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c409ac170dafe286e2cbd918b30a388.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c4147de069c1c7d819711e683fae373.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c4147de069c1c7d819711e683fae373.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d4be2d9edd8481dfa51cc7b86a90b36.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d4be2d9edd8481dfa51cc7b86a90b36.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61be18dbb282646133551c2bc297fb36.jpg\" _src=\"http://yanxuan.nosdn.127.net/61be18dbb282646133551c2bc297fb36.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7160604c5bd97a0f1aef7f3a2a32b72b.jpg\" _src=\"http://yanxuan.nosdn.127.net/7160604c5bd97a0f1aef7f3a2a32b72b.jpg\" style=\"\"/></p><p><br/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/32c5969b18a85bc62d4a855c40ab6142.jpg\" _src=\"http://yanxuan.nosdn.127.net/32c5969b18a85bc62d4a855c40ab6142.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62189479f43fd283340ce0fad3706b00.jpg\" _src=\"http://yanxuan.nosdn.127.net/62189479f43fd283340ce0fad3706b00.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f39cb441e6778d5d39510099f8befd3a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f39cb441e6778d5d39510099f8befd3a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bbb06c48c23cdf11fd93f711512eed7.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bbb06c48c23cdf11fd93f711512eed7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c0701aef423ba84cb1aabe8d6a1ab8d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/c0701aef423ba84cb1aabe8d6a1ab8d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4dec1e3bf4d5812d7d9fbddf50657e73.jpg\" _src=\"http://yanxuan.nosdn.127.net/4dec1e3bf4d5812d7d9fbddf50657e73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44497f9ad25cb6d208cc564016c8fd54.jpg\" _src=\"http://yanxuan.nosdn.127.net/44497f9ad25cb6d208cc564016c8fd54.jpg\"/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/37de0870b61ed6e880936d22000c2e85.jpg\" _src=\"http://yanxuan.nosdn.127.net/37de0870b61ed6e880936d22000c2e85.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97906141bd8846ea9e7888fa8a6b4ae0.jpg\" _src=\"http://yanxuan.nosdn.127.net/97906141bd8846ea9e7888fa8a6b4ae0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db23e00419f012686aaf4b3eeecae09b.jpg\" _src=\"http://yanxuan.nosdn.127.net/db23e00419f012686aaf4b3eeecae09b.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 24,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 1269,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/0d0a7e7d40a16ae6850d19f5e8704d8e.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/8b9328496990357033d4259fda250679.png",
      "retail_price": 899,
      "sell_volume": 205,
      "primary_product_id": 1029006,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "限时购",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 203,
      "is_hot": 0
    },
    {
      "id": 1030003,
      "category_id": 1008002,
      "goods_sn": "1030003",
      "name": "160*230羊毛手工几何地毯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "几何图案，打造立体的时尚感",
      "goods_desc": "<p><video id=\"tmpVedio0\" class=\"edui-upload-video video-js vjs-default-skin video-js\" controls=\"\" preload=\"auto\" width=\"100%\" height=\"\" data-setup=\"{}\"><source src=\"http://yanxuan.nosdn.127.net/e07746a58f5814648229ab750f7e59b0.mp4\" type=\"video/mp4\"/></video>‍</p><p><img src=\"http://yanxuan.nosdn.127.net/a03425edf97e1b0299d3095172991847.jpg\" _src=\"http://yanxuan.nosdn.127.net/a03425edf97e1b0299d3095172991847.jpg\" style=\"line-height: 1.42857;\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3fc35db4f3956b210032f0a876c2f2e.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3fc35db4f3956b210032f0a876c2f2e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf278ec3726e12e0a07ef4384f80d7c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf278ec3726e12e0a07ef4384f80d7c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/04cdc7e09537f67a140f5bd363751d23.jpg\" _src=\"http://yanxuan.nosdn.127.net/04cdc7e09537f67a140f5bd363751d23.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f4978e0569025d98c7a0cc685a3227d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/f4978e0569025d98c7a0cc685a3227d5.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/667999a8913e0dfc5118695f690f9ac4.jpg\" _src=\"http://yanxuan.nosdn.127.net/667999a8913e0dfc5118695f690f9ac4.jpg\" style=\"\"/></p><p><br/></p><p><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0fe6f158bf93e05ae12fbc86ad7df61.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0fe6f158bf93e05ae12fbc86ad7df61.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39b84d98bfcbc4f0443ec04e39328d04.jpg\" _src=\"http://yanxuan.nosdn.127.net/39b84d98bfcbc4f0443ec04e39328d04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16218f2ea0f8f4ddfd1fcbeac17d3b54.jpg\" _src=\"http://yanxuan.nosdn.127.net/16218f2ea0f8f4ddfd1fcbeac17d3b54.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e512605b0a5ee1dea333c42f826050b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e512605b0a5ee1dea333c42f826050b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/001d8961d92c3ebcf860e1745d0c63b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/001d8961d92c3ebcf860e1745d0c63b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25dda9b93dd3dd9aa622779c27481ef4.jpg\" _src=\"http://yanxuan.nosdn.127.net/25dda9b93dd3dd9aa622779c27481ef4.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/037abff9d64cdc761092d47619df82d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/037abff9d64cdc761092d47619df82d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f755e4142e8baf68fab301b3e6438d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f755e4142e8baf68fab301b3e6438d5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa9ac1211dca7edc8fd93efd9cdd66e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa9ac1211dca7edc8fd93efd9cdd66e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ada62ef76b083d844d0762d2a6d33824.jpg\" _src=\"http://yanxuan.nosdn.127.net/ada62ef76b083d844d0762d2a6d33824.jpg\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 23,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/d74913e762fa11a4e27b0a20b8dad02d.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/1d1ab099dc0e254c15e57302e78e200b.png",
      "retail_price": 1469,
      "sell_volume": 464,
      "primary_product_id": 1029008,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1035006,
      "category_id": 1008002,
      "goods_sn": "1035006",
      "name": "全棉单面割绒浴室地垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "手工制作，纯棉材质，柔软舒适",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/39cba017dbf04371863ec3af894cb79c.jpg\" _src=\"http://yanxuan.nosdn.127.net/39cba017dbf04371863ec3af894cb79c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/727bdb71768265b3c283b2d71ad63d8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/727bdb71768265b3c283b2d71ad63d8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b7eb8df6b30b61ff8326a5882bbf411.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b7eb8df6b30b61ff8326a5882bbf411.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5143f756b613c2523954affbdf514a05.jpg\" _src=\"http://yanxuan.nosdn.127.net/5143f756b613c2523954affbdf514a05.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5a6879162b60e2442036c6c5d88275e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/5a6879162b60e2442036c6c5d88275e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d65d49dfd73f6b44d8e1b971df58ec1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/d65d49dfd73f6b44d8e1b971df58ec1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/630c9a177eb89c044d4c968745fce915.jpg\" _src=\"http://yanxuan.nosdn.127.net/630c9a177eb89c044d4c968745fce915.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1597a314b6ae69f361f4f1fbc2ed876c.jpg\" _src=\"http://yanxuan.nosdn.127.net/1597a314b6ae69f361f4f1fbc2ed876c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cfcfff37b305dcc44d9a907377761f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cfcfff37b305dcc44d9a907377761f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27dd23d01d9d110ebb11c92fa087e208.jpg\" _src=\"http://yanxuan.nosdn.127.net/27dd23d01d9d110ebb11c92fa087e208.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/366f5281836ad5b3a06afe4ace14d2bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/366f5281836ad5b3a06afe4ace14d2bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cdd2229692184db4793f68ca2d1c307.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cdd2229692184db4793f68ca2d1c307.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/999c7854dff1496c2702c510b8c6586d.jpg\" _src=\"http://yanxuan.nosdn.127.net/999c7854dff1496c2702c510b8c6586d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7097f2a9c69c4f337ab9ff961276cf0a.jpg\" _src=\"http://yanxuan.nosdn.127.net/7097f2a9c69c4f337ab9ff961276cf0a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d6ad8caac9c24f024b9525e492dde1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d6ad8caac9c24f024b9525e492dde1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1005834f8ac736dc7bc5c59cfab0ce01.jpg\" _src=\"http://yanxuan.nosdn.127.net/1005834f8ac736dc7bc5c59cfab0ce01.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/342365052bc031f64050c0d117786de1.jpg\" _src=\"http://yanxuan.nosdn.127.net/342365052bc031f64050c0d117786de1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bdb057b4b109ad39368d337b26fcef0.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bdb057b4b109ad39368d337b26fcef0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c764541e44c1bfe9308c4be9ba70eb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c764541e44c1bfe9308c4be9ba70eb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e4dafc25a731ccf56b1296e9889530d.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e4dafc25a731ccf56b1296e9889530d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0aae3c93d54fd9a25fc0d297e0cf856e.jpg\" _src=\"http://yanxuan.nosdn.127.net/0aae3c93d54fd9a25fc0d297e0cf856e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d3f4adea81508c83148517b12b3963f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d3f4adea81508c83148517b12b3963f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a7f792a547c9f534fd4bd00c88fe734c.jpg\" _src=\"http://yanxuan.nosdn.127.net/a7f792a547c9f534fd4bd00c88fe734c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41541dc15fbb715ed5311d4343516a6e.jpg\" _src=\"http://yanxuan.nosdn.127.net/41541dc15fbb715ed5311d4343516a6e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/267175ffcb24b51250f642b31cadd977.jpg\" _src=\"http://yanxuan.nosdn.127.net/267175ffcb24b51250f642b31cadd977.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 32,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 69,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/96b3f9af4a260902e7b8b3100af1da07.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ee92704f3b8323905b51fc647823e6e5.png",
      "retail_price": 56,
      "sell_volume": 14584,
      "primary_product_id": 1034011,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "限时购",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 203,
      "is_hot": 0
    },
    {
      "id": 1039051,
      "category_id": 1008002,
      "goods_sn": "1039051",
      "name": "多功能午睡枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "放松自在的午后时光",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/aba5fac220a511eb859ad4834fd7c0e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/aba5fac220a511eb859ad4834fd7c0e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37c7411fe03ac22b8b924190a5c6f483.jpg\" _src=\"http://yanxuan.nosdn.127.net/37c7411fe03ac22b8b924190a5c6f483.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88e313d81b848936d673edebc823f617.jpg\" _src=\"http://yanxuan.nosdn.127.net/88e313d81b848936d673edebc823f617.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/efddbb9e7105a72fb40f168813764297.jpg\" _src=\"http://yanxuan.nosdn.127.net/efddbb9e7105a72fb40f168813764297.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4830e1927e472f45940a92acf3e04331.jpg\" _src=\"http://yanxuan.nosdn.127.net/4830e1927e472f45940a92acf3e04331.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10b2f2989c7239bcea42be91d1826fc7.jpg\" _src=\"http://yanxuan.nosdn.127.net/10b2f2989c7239bcea42be91d1826fc7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3d19a5320eb179b3752458f15f1a068.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3d19a5320eb179b3752458f15f1a068.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97a9d81d01cbc6c8bf57e8b308de1537.jpg\" _src=\"http://yanxuan.nosdn.127.net/97a9d81d01cbc6c8bf57e8b308de1537.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/500497dcf877fbf29548ef7eae7766fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/500497dcf877fbf29548ef7eae7766fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92f6105f284bdd94aa4b6495a7d43994.jpg\" _src=\"http://yanxuan.nosdn.127.net/92f6105f284bdd94aa4b6495a7d43994.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60161ebc38b0b8c8ca9de8a0165843bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/60161ebc38b0b8c8ca9de8a0165843bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ce9817e2d4415c5789028c57c593450.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ce9817e2d4415c5789028c57c593450.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e3dc4f7c9dcd228a94cc4ffa6cea1be.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e3dc4f7c9dcd228a94cc4ffa6cea1be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89360198abf4bbb4c108bfe1068d83b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/89360198abf4bbb4c108bfe1068d83b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f40b5ba3618e61e80ad8f175b3da866.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f40b5ba3618e61e80ad8f175b3da866.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad590b8d9cb20c046d0d8e68ea3b0dc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad590b8d9cb20c046d0d8e68ea3b0dc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c606522a6032f1a2268a0ee0d8d01dff.jpg\" _src=\"http://yanxuan.nosdn.127.net/c606522a6032f1a2268a0ee0d8d01dff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f226b9e158f2cf451e925a606d1b5ecd.jpg\" _src=\"http://yanxuan.nosdn.127.net/f226b9e158f2cf451e925a606d1b5ecd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b169357e50d02d557c468588939c7f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b169357e50d02d557c468588939c7f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5e676b79ffc838a2c496134c8c3f55f.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5e676b79ffc838a2c496134c8c3f55f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e934b380901ffa4b035825b82246634e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e934b380901ffa4b035825b82246634e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8decfed210a7ada28bd71496a8ef51a.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8decfed210a7ada28bd71496a8ef51a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fcc94c2ee6ea13ef7cd7d21f1c63b79.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fcc94c2ee6ea13ef7cd7d21f1c63b79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8bae5453415f2fd519b5cf836e9baddc.jpg\" _src=\"http://yanxuan.nosdn.127.net/8bae5453415f2fd519b5cf836e9baddc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5833f7b80c040d8bdf23e514d430e045.jpg\" _src=\"http://yanxuan.nosdn.127.net/5833f7b80c040d8bdf23e514d430e045.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15df0095ff692e8d67185c93c44680c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/15df0095ff692e8d67185c93c44680c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32fdd19de26dee3281e76dc33059b1f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/32fdd19de26dee3281e76dc33059b1f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/290d679b2fe2154ef36b777525d988bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/290d679b2fe2154ef36b777525d988bc.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99233a211060d951818a729d43bb6533.jpg\" _src=\"http://yanxuan.nosdn.127.net/99233a211060d951818a729d43bb6533.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76fcb532c1aa2f631c0e439f5986654f.jpg\" _src=\"http://yanxuan.nosdn.127.net/76fcb532c1aa2f631c0e439f5986654f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2e90d2089e907d605e1eee0e6fcb1d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2e90d2089e907d605e1eee0e6fcb1d1.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 14,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/20e7e05935a347b36adac369efc490c3.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/c8ca0600fa7ba11ca8be6a3173dd38c9.png",
      "retail_price": 79,
      "sell_volume": 8202,
      "primary_product_id": 1038068,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1043005,
      "category_id": 1008002,
      "goods_sn": "1043005",
      "name": "日式记忆绵坐垫",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "活性炭记忆绵，缓解压力",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/7239e35762ea2937549f53f4482124fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/7239e35762ea2937549f53f4482124fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c23c022ad6737aa351140d7ce97a4a43.jpg\" _src=\"http://yanxuan.nosdn.127.net/c23c022ad6737aa351140d7ce97a4a43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b6fe3f499101077e6ee595a9145172c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b6fe3f499101077e6ee595a9145172c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fdc843045b99838abd8ce3fcbec2890.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fdc843045b99838abd8ce3fcbec2890.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14d3e1c384f5bc66e85b4dfff61f49ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/14d3e1c384f5bc66e85b4dfff61f49ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14eed3d4524fe441a54b604f37cfd299.jpg\" _src=\"http://yanxuan.nosdn.127.net/14eed3d4524fe441a54b604f37cfd299.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1b3a30c34e6fecf8105bf430e6d547f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1b3a30c34e6fecf8105bf430e6d547f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb5411b150ce5a69c0f88ef3af918061.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb5411b150ce5a69c0f88ef3af918061.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aebe8243acfa28a42d300d985c6e7036.jpg\" _src=\"http://yanxuan.nosdn.127.net/aebe8243acfa28a42d300d985c6e7036.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1371f124f86fc38c195f49e4bf26ddc5.jpg\" _src=\"http://yanxuan.nosdn.127.net/1371f124f86fc38c195f49e4bf26ddc5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd05471ebf5529464c85eace3e7c5c7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd05471ebf5529464c85eace3e7c5c7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c607e963758e4ad3f3bc749098fdcec.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c607e963758e4ad3f3bc749098fdcec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd472e779f1748937d269b87464722b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd472e779f1748937d269b87464722b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d19ec3e68922cdae4da8c0ab174bf5eb.jpg\" _src=\"http://yanxuan.nosdn.127.net/d19ec3e68922cdae4da8c0ab174bf5eb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44003fe38ab817003cb441ed5e518c41.jpg\" _src=\"http://yanxuan.nosdn.127.net/44003fe38ab817003cb441ed5e518c41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f3a7c45c70930950e60ddac979953d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f3a7c45c70930950e60ddac979953d5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77fc74a83c328dddf610a045277f094e.jpg\" _src=\"http://yanxuan.nosdn.127.net/77fc74a83c328dddf610a045277f094e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14056056c8e8cf3f77a479de696d18ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/14056056c8e8cf3f77a479de696d18ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ec2764b8b29c67af332cc1fde825b70.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ec2764b8b29c67af332cc1fde825b70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/494504fdb2d59d924de16cf79629dee9.jpg\" _src=\"http://yanxuan.nosdn.127.net/494504fdb2d59d924de16cf79629dee9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddf59afdada25b6b7aad72aaf8f0af20.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddf59afdada25b6b7aad72aaf8f0af20.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b8ad80c319aac920f3409bcd4376e17.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b8ad80c319aac920f3409bcd4376e17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8571525a4f280d09926a1b388d06fe8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/8571525a4f280d09926a1b388d06fe8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23c8bb2834f9ec05adb69e4df8354224.jpg\" _src=\"http://yanxuan.nosdn.127.net/23c8bb2834f9ec05adb69e4df8354224.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9c44aea67b0392547fdb3ba7f24c5fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9c44aea67b0392547fdb3ba7f24c5fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5045464902396b85ea12724ed962d7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5045464902396b85ea12724ed962d7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f484b21d07738839d1e199d8ba1031f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/f484b21d07738839d1e199d8ba1031f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21718c637256576c66876aa30653e29d.jpg\" _src=\"http://yanxuan.nosdn.127.net/21718c637256576c66876aa30653e29d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 11,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/aedfe3b7d76361d104a425ff551ade77.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/2a95b16f5b147cab4845641bee738a2e.png",
      "retail_price": 59,
      "sell_volume": 7482,
      "primary_product_id": 1041015,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1048005,
      "category_id": 1008002,
      "goods_sn": "1048005",
      "name": "日式色织水洗条纹抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "色织面料，水洗工艺，柔软亲肤",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/39afc6f165cf752e16c199b65ab61ee8.jpg\" _src=\"http://yanxuan.nosdn.127.net/39afc6f165cf752e16c199b65ab61ee8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2635f2eb08e98687a132a97642d87de.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2635f2eb08e98687a132a97642d87de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08b6bca750a85d833740e1f12e5a6216.jpg\" _src=\"http://yanxuan.nosdn.127.net/08b6bca750a85d833740e1f12e5a6216.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f61f9587dc8aec8330335da87dbb60ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/f61f9587dc8aec8330335da87dbb60ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f22282ebbbeb664ba706e4f088c9db2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/f22282ebbbeb664ba706e4f088c9db2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad7819c5597db9fce742cbc61aa53c72.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad7819c5597db9fce742cbc61aa53c72.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ee4a43824784e660f44e16274c4717ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/ee4a43824784e660f44e16274c4717ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f0eb752fd857fa1af74602afadabb0fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/f0eb752fd857fa1af74602afadabb0fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/46290c0b824babab46ce73feb23a554d.jpg\" _src=\"http://yanxuan.nosdn.127.net/46290c0b824babab46ce73feb23a554d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1c34134e19df505b4b1b2277880bba2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1c34134e19df505b4b1b2277880bba2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0bce553f09f5146ba9209264c46e38ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/0bce553f09f5146ba9209264c46e38ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/732ed69a0539f4d972213ed64e5bcff0.jpg\" _src=\"http://yanxuan.nosdn.127.net/732ed69a0539f4d972213ed64e5bcff0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/147fcd503618a36a76ed792c6a2254b1.jpg\" _src=\"http://yanxuan.nosdn.127.net/147fcd503618a36a76ed792c6a2254b1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f68cea7d1e7dd23349f7c36e366cb6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f68cea7d1e7dd23349f7c36e366cb6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/852711207b87360d29289be16a76e5ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/852711207b87360d29289be16a76e5ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f46c1d0edb91be4fa7c2747b423c494.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f46c1d0edb91be4fa7c2747b423c494.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f2bc29d55899694b917c9991d0b1333.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f2bc29d55899694b917c9991d0b1333.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63d4fa2caa8bbd1d7e205e90fe176633.jpg\" _src=\"http://yanxuan.nosdn.127.net/63d4fa2caa8bbd1d7e205e90fe176633.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f885db84f7911c3c4abc9695f55f19f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/f885db84f7911c3c4abc9695f55f19f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd0c5be6c986a60a577ab7fd4fa9796e.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd0c5be6c986a60a577ab7fd4fa9796e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb0f814679347c4876f2ca30acd57f88.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb0f814679347c4876f2ca30acd57f88.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/64b5936ea7e076885a7c1611d492aa57.jpg\" _src=\"http://yanxuan.nosdn.127.net/64b5936ea7e076885a7c1611d492aa57.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b503dd5b259a049dc3fffcabe6264c10.jpg\" _src=\"http://yanxuan.nosdn.127.net/b503dd5b259a049dc3fffcabe6264c10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3fb47a70640f6c252518a80a803bd362.jpg\" _src=\"http://yanxuan.nosdn.127.net/3fb47a70640f6c252518a80a803bd362.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1837c9a132b1ca0ed52f76f935563b7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1837c9a132b1ca0ed52f76f935563b7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09e9cc037e909c934aba0b87c48914ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/09e9cc037e909c934aba0b87c48914ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5c3a85ee4217386a8161016aa7727b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5c3a85ee4217386a8161016aa7727b9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e666622ecebc8fc733a49c5ad7d16c3e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e666622ecebc8fc733a49c5ad7d16c3e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48f87049ad7e2492ae75da78b97cd6fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/48f87049ad7e2492ae75da78b97cd6fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21cc4790d10496f2e73531c420fbb394.jpg\" _src=\"http://yanxuan.nosdn.127.net/21cc4790d10496f2e73531c420fbb394.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9510a74920b5589cba7af910774f8c0c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9510a74920b5589cba7af910774f8c0c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c69b713c98187890316668d10aa55c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c69b713c98187890316668d10aa55c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dcafde6d38fd075c4ba6d0cc1e816314.jpg\" _src=\"http://yanxuan.nosdn.127.net/dcafde6d38fd075c4ba6d0cc1e816314.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ccdf51824645c27ab06e78faa85db7d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ccdf51824645c27ab06e78faa85db7d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8096a502cac9f926d288cbbe8b8534fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/8096a502cac9f926d288cbbe8b8534fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b2b9a1f8a1422e3975cbee85685672c.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b2b9a1f8a1422e3975cbee85685672c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fd6779619cc7ed6f2a4057526f0c579d.jpg\" _src=\"http://yanxuan.nosdn.127.net/fd6779619cc7ed6f2a4057526f0c579d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdef4d1620407043511daf2e97746f07.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdef4d1620407043511daf2e97746f07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f30d798c772ea1599723c427c1d643b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f30d798c772ea1599723c427c1d643b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0cfc9aae9304010e24d92b29220dc0b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/0cfc9aae9304010e24d92b29220dc0b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e20e47f1eaf643bc569ccb148781529.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e20e47f1eaf643bc569ccb148781529.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9beb4226eb47be1c16e872dd9281634.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9beb4226eb47be1c16e872dd9281634.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70d2d737fbf7fc5980604ea294942b41.jpg\" _src=\"http://yanxuan.nosdn.127.net/70d2d737fbf7fc5980604ea294942b41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/496224b05a3054625b065de6aa769959.jpg\" _src=\"http://yanxuan.nosdn.127.net/496224b05a3054625b065de6aa769959.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0671941e0dfb696d5392f174a949a13.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0671941e0dfb696d5392f174a949a13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2df72e131e86e433d939776783a44db7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2df72e131e86e433d939776783a44db7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3bea99ca3040befe69d4811e0ef9b226.jpg\" _src=\"http://yanxuan.nosdn.127.net/3bea99ca3040befe69d4811e0ef9b226.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbc003f18889ab46a5a3a7e8698df351.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbc003f18889ab46a5a3a7e8698df351.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ee0df8d583844e734273d73eb582a4a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ee0df8d583844e734273d73eb582a4a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ea9467e6f4ef5c8f0812c1595704840.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ea9467e6f4ef5c8f0812c1595704840.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 5,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2167445c1b3df028d660bb992f321396.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ce980c16810a471dffff6aa8d7bac754.png",
      "retail_price": 59,
      "sell_volume": 5846,
      "primary_product_id": 1047014,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1055012,
      "category_id": 1008002,
      "goods_sn": "1055012",
      "name": "300根全棉羽丝绒抱枕芯",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "仪征3D填充，充实的满足感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/07f2717762df73a6a697bb5399da6376.jpg\" _src=\"http://yanxuan.nosdn.127.net/07f2717762df73a6a697bb5399da6376.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e202bdb4be8f36bda118cf7265d00f65.jpg\" _src=\"http://yanxuan.nosdn.127.net/e202bdb4be8f36bda118cf7265d00f65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b5766cf268d327a3518ee5429c4c4e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b5766cf268d327a3518ee5429c4c4e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f4e4356d070dbca22cf19a60a2447ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f4e4356d070dbca22cf19a60a2447ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da3a3e22d355ccf82235603507f3a083.jpg\" _src=\"http://yanxuan.nosdn.127.net/da3a3e22d355ccf82235603507f3a083.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be789777e5e1381bb7b62d26fcfb619e.jpg\" _src=\"http://yanxuan.nosdn.127.net/be789777e5e1381bb7b62d26fcfb619e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c48e78aa87b8e81eab6a60de74d1c19c.jpg\" _src=\"http://yanxuan.nosdn.127.net/c48e78aa87b8e81eab6a60de74d1c19c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f772f4990d8ae0acac660acf25be2d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f772f4990d8ae0acac660acf25be2d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f1bd930fcb57e79a4ce2a1c4a0f2f4c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f1bd930fcb57e79a4ce2a1c4a0f2f4c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f481e1e9b8c4e728f4f7225af52a335e.jpg\" _src=\"http://yanxuan.nosdn.127.net/f481e1e9b8c4e728f4f7225af52a335e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4fca69439b053b510724cf6834856a2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/4fca69439b053b510724cf6834856a2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a285ec5ac9c84a6616feca7301f515c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a285ec5ac9c84a6616feca7301f515c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52435458ac1c48fb45f4a9888052b5b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/52435458ac1c48fb45f4a9888052b5b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/01301675d00e13d21588d0bbb72e1745.jpg\" _src=\"http://yanxuan.nosdn.127.net/01301675d00e13d21588d0bbb72e1745.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63627106753f764733cf47047e887d1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/63627106753f764733cf47047e887d1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15ecf40c8045513fe6a1303fe7d4383f.jpg\" _src=\"http://yanxuan.nosdn.127.net/15ecf40c8045513fe6a1303fe7d4383f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e8ef113464ff066662e639868e6eda28.jpg\" _src=\"http://yanxuan.nosdn.127.net/e8ef113464ff066662e639868e6eda28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0de1977400dfda99d0601e1c12fdbf1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/0de1977400dfda99d0601e1c12fdbf1e.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 10,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/06930cbd3bcd7c98d7740c18a7986137.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/3d437c8d68e2ec3f3dd61001bf98f16e.png",
      "retail_price": 39,
      "sell_volume": 6669,
      "primary_product_id": 1056022,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1055016,
      "category_id": 1008002,
      "goods_sn": "1055016",
      "name": "日式纯棉针织条纹抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "亲肤舒适，宛如妈妈的怀抱",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/4060bcde249c2501e5d95cfa0888a6c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/4060bcde249c2501e5d95cfa0888a6c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afebd965217cfdbc238de9252c7d6e37.jpg\" _src=\"http://yanxuan.nosdn.127.net/afebd965217cfdbc238de9252c7d6e37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b017649229c04dad59c312b3fe0cf7be.jpg\" _src=\"http://yanxuan.nosdn.127.net/b017649229c04dad59c312b3fe0cf7be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e02d923a92d5bef4b264381cffd5d813.jpg\" _src=\"http://yanxuan.nosdn.127.net/e02d923a92d5bef4b264381cffd5d813.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0447366651e06dde345c907e12315c73.jpg\" _src=\"http://yanxuan.nosdn.127.net/0447366651e06dde345c907e12315c73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5fdb8a54a2bc2285d1136bf9a2a674f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5fdb8a54a2bc2285d1136bf9a2a674f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1836dd3b75444a3ce42dc49fa5ee513.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1836dd3b75444a3ce42dc49fa5ee513.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f4740ae47c3ca8465e1ea6ec0a43563.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f4740ae47c3ca8465e1ea6ec0a43563.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f9f33a85933788209e6195468044387.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f9f33a85933788209e6195468044387.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b6ceab4330e0dd218db3c16582465be1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b6ceab4330e0dd218db3c16582465be1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dea7df197ba1e5ce5e9646aea43f798.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dea7df197ba1e5ce5e9646aea43f798.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/022e305413c9aa8e8db30a46a2a65286.jpg\" _src=\"http://yanxuan.nosdn.127.net/022e305413c9aa8e8db30a46a2a65286.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cce2571a59a0bc39784d61c4134f9458.jpg\" _src=\"http://yanxuan.nosdn.127.net/cce2571a59a0bc39784d61c4134f9458.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1f287dab80d1b11450051de6c119611.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1f287dab80d1b11450051de6c119611.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7b6318cb7623349542ba971cf1887da.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7b6318cb7623349542ba971cf1887da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf56a8ae91e07c91d70cf7b88cb59676.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf56a8ae91e07c91d70cf7b88cb59676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76aebdbc4a150837b2dcaa2293c85cc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/76aebdbc4a150837b2dcaa2293c85cc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/902fb302066a65488ed1f6da3a16ed66.jpg\" _src=\"http://yanxuan.nosdn.127.net/902fb302066a65488ed1f6da3a16ed66.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd9df2852e760940b0ab9e599320ed35.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd9df2852e760940b0ab9e599320ed35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ad1c6c9e619df09685cf9596339d714.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ad1c6c9e619df09685cf9596339d714.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83e54a3b9d13dc3c67e880c02e63167c.jpg\" _src=\"http://yanxuan.nosdn.127.net/83e54a3b9d13dc3c67e880c02e63167c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f6b75fe4ff9ae0b976c8c85bbf0a719.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f6b75fe4ff9ae0b976c8c85bbf0a719.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82f850ea52ca3e7048283b3f8a65c616.jpg\" _src=\"http://yanxuan.nosdn.127.net/82f850ea52ca3e7048283b3f8a65c616.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5bd4faa4898d9ea3c56fba9c5749cc62.jpg\" _src=\"http://yanxuan.nosdn.127.net/5bd4faa4898d9ea3c56fba9c5749cc62.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6488dedf51c6e5a90fc5f156a4e8416b.jpg\" _src=\"http://yanxuan.nosdn.127.net/6488dedf51c6e5a90fc5f156a4e8416b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bc667ddb5116ceaf329f55982da36bb1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bc667ddb5116ceaf329f55982da36bb1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfbfde943773a0258fa81b84d710d36e.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfbfde943773a0258fa81b84d710d36e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60d64bb0ac51346dc39d266beacdb846.jpg\" _src=\"http://yanxuan.nosdn.127.net/60d64bb0ac51346dc39d266beacdb846.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c50c0fd364d6b9a8646d0da75ce48f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c50c0fd364d6b9a8646d0da75ce48f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b24da9df819efdf9e110bb2228eadf0d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b24da9df819efdf9e110bb2228eadf0d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3cbbd9ec8dd41be2b35bf49842b67d86.jpg\" _src=\"http://yanxuan.nosdn.127.net/3cbbd9ec8dd41be2b35bf49842b67d86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d5bb53b92ed48f3f81980e41b51c0fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d5bb53b92ed48f3f81980e41b51c0fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d75a8fd77357f9a74a36fd7bfa7cebed.jpg\" _src=\"http://yanxuan.nosdn.127.net/d75a8fd77357f9a74a36fd7bfa7cebed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2dd8069e6739d732a53c25c74c0b2a89.jpg\" _src=\"http://yanxuan.nosdn.127.net/2dd8069e6739d732a53c25c74c0b2a89.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d7b4e172f8fd168e28854c3d8d04c56f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d7b4e172f8fd168e28854c3d8d04c56f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8b981b58ffb3e0a75916def11e45493.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8b981b58ffb3e0a75916def11e45493.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fb12dd3d12c8828a5cf2e16f17a8f27.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fb12dd3d12c8828a5cf2e16f17a8f27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8df57201eb9f5e7b576a6ccc31286e8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8df57201eb9f5e7b576a6ccc31286e8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f86f20ab83206abfdd682418e3cd3ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f86f20ab83206abfdd682418e3cd3ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c64ea783c9bd6dd2cb51b9978769edb.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c64ea783c9bd6dd2cb51b9978769edb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/104dca8bdfb6413fed5379a5b04eec10.jpg\" _src=\"http://yanxuan.nosdn.127.net/104dca8bdfb6413fed5379a5b04eec10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2cfb7760b81f0a82bdbae5079bfcd5ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/2cfb7760b81f0a82bdbae5079bfcd5ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1c6e09984c0599b5205f4d099cd5cfcb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1c6e09984c0599b5205f4d099cd5cfcb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e32f3a0bbc7ba3ec49b69fa89ba7da39.jpg\" _src=\"http://yanxuan.nosdn.127.net/e32f3a0bbc7ba3ec49b69fa89ba7da39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/408bf6b2815efea1020278ff57204667.jpg\" _src=\"http://yanxuan.nosdn.127.net/408bf6b2815efea1020278ff57204667.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6707b10b7a14f7d2e7487f30a687cfb2.jpg\" _src=\"http://yanxuan.nosdn.127.net/6707b10b7a14f7d2e7487f30a687cfb2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c4977d2ce8691f85575698990c13c3a.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c4977d2ce8691f85575698990c13c3a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22213164e3ce12c23260519cc5f2dd7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/22213164e3ce12c23260519cc5f2dd7f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9c8f7fda81f79cec8e75404386677c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9c8f7fda81f79cec8e75404386677c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1e5093b54f817ed1906fc58e7494790.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1e5093b54f817ed1906fc58e7494790.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/162452d2cb5ad3348862d5b1da7348c5.jpg\" _src=\"http://yanxuan.nosdn.127.net/162452d2cb5ad3348862d5b1da7348c5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8f6de9bc947bed7d5cebfe1f49a786d.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8f6de9bc947bed7d5cebfe1f49a786d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 8,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/8132003a8940c7056960c3c5fce59903.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/23e0203f1512f33e605f61c28fa03d2d.png",
      "retail_price": 59,
      "sell_volume": 948,
      "primary_product_id": 1056032,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1057036,
      "category_id": 1008002,
      "goods_sn": "1057036",
      "name": "日式纯色水洗亚麻抱枕",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "水洗亚麻，透气亲肤",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/6b69f7597ccffd27d77467d9d04eb294.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b69f7597ccffd27d77467d9d04eb294.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a89ca371ef07355c1feb293db961bd30.jpg\" _src=\"http://yanxuan.nosdn.127.net/a89ca371ef07355c1feb293db961bd30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2076e89c5f8fde4f44f918bd02d18eb7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2076e89c5f8fde4f44f918bd02d18eb7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5c9111e4dcc13cb41db98f68086cc620.jpg\" _src=\"http://yanxuan.nosdn.127.net/5c9111e4dcc13cb41db98f68086cc620.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f0645abcf883e7a863f32ce95f3c26b.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f0645abcf883e7a863f32ce95f3c26b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76a2b12f2d0f48f268d18b0ca0d1d6bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/76a2b12f2d0f48f268d18b0ca0d1d6bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a91f75159867f33a91f4e9992e00afa1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a91f75159867f33a91f4e9992e00afa1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93de61256a8ff3a8aa4bb90847ff454e.jpg\" _src=\"http://yanxuan.nosdn.127.net/93de61256a8ff3a8aa4bb90847ff454e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f611f99bea2920881e1421c110970234.jpg\" _src=\"http://yanxuan.nosdn.127.net/f611f99bea2920881e1421c110970234.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a292339423f141ad5d7a4011ea316956.jpg\" _src=\"http://yanxuan.nosdn.127.net/a292339423f141ad5d7a4011ea316956.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2045ae4f861d9eae6af351b9d82c9239.jpg\" _src=\"http://yanxuan.nosdn.127.net/2045ae4f861d9eae6af351b9d82c9239.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/398718a6d579c4af5f255909283e44a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/398718a6d579c4af5f255909283e44a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5be95e2db627908d23605fe042af2937.jpg\" _src=\"http://yanxuan.nosdn.127.net/5be95e2db627908d23605fe042af2937.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50a4fa0f67aa85dfaad36695225fe2f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/50a4fa0f67aa85dfaad36695225fe2f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c825e297cfbaaae632146a55c61dc3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c825e297cfbaaae632146a55c61dc3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/261c7819e7e9ac165e64cae88a59f70c.jpg\" _src=\"http://yanxuan.nosdn.127.net/261c7819e7e9ac165e64cae88a59f70c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec83f40d91fcc79f59a2479dffeb4565.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec83f40d91fcc79f59a2479dffeb4565.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/26f3e85402086b7d261a650e244dc676.jpg\" _src=\"http://yanxuan.nosdn.127.net/26f3e85402086b7d261a650e244dc676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dccb68f0d97112d245ab1924744b94b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/dccb68f0d97112d245ab1924744b94b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaba69949efd7ed85e72071f4ade4945.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaba69949efd7ed85e72071f4ade4945.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f23300061e5cf871e86a51f0012e885.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f23300061e5cf871e86a51f0012e885.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a55eedca057e0c973549ac8f13b47800.jpg\" _src=\"http://yanxuan.nosdn.127.net/a55eedca057e0c973549ac8f13b47800.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abf16e831285e3d97dbb60a3162e7968.jpg\" _src=\"http://yanxuan.nosdn.127.net/abf16e831285e3d97dbb60a3162e7968.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9390c8dab9fc7d8c27ac9410eb0340c.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9390c8dab9fc7d8c27ac9410eb0340c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8feb2be5afec5abe439cf1b42683373f.jpg\" _src=\"http://yanxuan.nosdn.127.net/8feb2be5afec5abe439cf1b42683373f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/beb7620d0f685ab9c3af7ed18284b29e.jpg\" _src=\"http://yanxuan.nosdn.127.net/beb7620d0f685ab9c3af7ed18284b29e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f70ceed2078d44d747a9ce369feee9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f70ceed2078d44d747a9ce369feee9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5469e219bd5347568337746b257f094e.jpg\" _src=\"http://yanxuan.nosdn.127.net/5469e219bd5347568337746b257f094e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a177a6b6e58580809330895ebdbaff6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/a177a6b6e58580809330895ebdbaff6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9db0090d56ab757babb2ba661726cbe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/9db0090d56ab757babb2ba661726cbe3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6363637e0dd2fc670745c217b2a5cbfc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6363637e0dd2fc670745c217b2a5cbfc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1af1bde98f1497f591f62bff99ccca54.jpg\" _src=\"http://yanxuan.nosdn.127.net/1af1bde98f1497f591f62bff99ccca54.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69d034b353ae2e6e30afb6c21483690f.jpg\" _src=\"http://yanxuan.nosdn.127.net/69d034b353ae2e6e30afb6c21483690f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e29d6ac5ed040d63847ca456a179d43.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e29d6ac5ed040d63847ca456a179d43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29e460fba57f67cd83121f6cb917cfbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/29e460fba57f67cd83121f6cb917cfbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16090c02f4d4b76c6be82d98e489586e.jpg\" _src=\"http://yanxuan.nosdn.127.net/16090c02f4d4b76c6be82d98e489586e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c840eb66cf002227c52a13fbe55f657b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c840eb66cf002227c52a13fbe55f657b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16f65265b0942a60f3241704dc29be13.jpg\" _src=\"http://yanxuan.nosdn.127.net/16f65265b0942a60f3241704dc29be13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54a63da54b4e80867d8cd92d1ea9576e.jpg\" _src=\"http://yanxuan.nosdn.127.net/54a63da54b4e80867d8cd92d1ea9576e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebd0b906076850983e5a2aae9f667ce7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebd0b906076850983e5a2aae9f667ce7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bbf32cdc82643a85c12ff05ea88088ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/bbf32cdc82643a85c12ff05ea88088ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca6e3ccc3725c3f58338b62a5a0655d3.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca6e3ccc3725c3f58338b62a5a0655d3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ef02962e6155f811566aad168dabbec.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ef02962e6155f811566aad168dabbec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/832735166071f05288ffd347dff58ee6.jpg\" _src=\"http://yanxuan.nosdn.127.net/832735166071f05288ffd347dff58ee6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4fc490c4e9a0a0fa0affd317b8526f4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4fc490c4e9a0a0fa0affd317b8526f4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b05f975f16c09f106c81533c1a249b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b05f975f16c09f106c81533c1a249b0.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 6,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/f40fffd36cc85d5e0cf69417f4192ac1.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/8a9ee5ba08929cc9e40b973607d2f633.png",
      "retail_price": 79,
      "sell_volume": 1727,
      "primary_product_id": 1058097,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1072000,
      "category_id": 1008002,
      "goods_sn": "1072000",
      "name": "手工针织绞花抱枕套",
      "brand_id": 1001020,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "纯手工针织，带给你复古的暖",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/74ead5d764e22f8d50dc44a7a61da41a.jpg\" _src=\"http://yanxuan.nosdn.127.net/74ead5d764e22f8d50dc44a7a61da41a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be7f775d658e40e6ca76e657006053a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/be7f775d658e40e6ca76e657006053a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7fe9345385034a4d25580072444b349b.jpg\" _src=\"http://yanxuan.nosdn.127.net/7fe9345385034a4d25580072444b349b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bffafbafcf3010c3e5ab454af09cde4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/bffafbafcf3010c3e5ab454af09cde4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/123a0dcb707c2a178e5f9da395b5b24e.jpg\" _src=\"http://yanxuan.nosdn.127.net/123a0dcb707c2a178e5f9da395b5b24e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfeba71e7e71a63dee06b079b4c4c4f0.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfeba71e7e71a63dee06b079b4c4c4f0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cdc034602358c7752073a9b4bd6b499f.jpg\" _src=\"http://yanxuan.nosdn.127.net/cdc034602358c7752073a9b4bd6b499f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3050a816fd41ec2b8880d11aafc26177.jpg\" _src=\"http://yanxuan.nosdn.127.net/3050a816fd41ec2b8880d11aafc26177.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/027e8c218edbbf1779cf4b380b2133c2.jpg\" _src=\"http://yanxuan.nosdn.127.net/027e8c218edbbf1779cf4b380b2133c2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbd1f6dd39bd517c99c7ae07d9b32b0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbd1f6dd39bd517c99c7ae07d9b32b0e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db5baa7586787b7e0f27a5b7a09946a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/db5baa7586787b7e0f27a5b7a09946a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/66a0ff102559b2d840240d6fa8c37001.jpg\" _src=\"http://yanxuan.nosdn.127.net/66a0ff102559b2d840240d6fa8c37001.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b17b0772d947612819e4489d9e5a865.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b17b0772d947612819e4489d9e5a865.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53cc65ea58a7757fca2585b25056cf21.jpg\" _src=\"http://yanxuan.nosdn.127.net/53cc65ea58a7757fca2585b25056cf21.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/86506725ae85f9864c8b70b64b2e37d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/86506725ae85f9864c8b70b64b2e37d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/671d390a50d363d6ae6ab0c52f06a284.jpg\" _src=\"http://yanxuan.nosdn.127.net/671d390a50d363d6ae6ab0c52f06a284.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14e864b84a51faebab51912bbfea7b75.jpg\" _src=\"http://yanxuan.nosdn.127.net/14e864b84a51faebab51912bbfea7b75.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e31d1086f08b77298977c2b459be4833.jpg\" _src=\"http://yanxuan.nosdn.127.net/e31d1086f08b77298977c2b459be4833.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02338b650755a458ca8561f484e618d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/02338b650755a458ca8561f484e618d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ffbeafbda15fcfcf98c3b7a62c77e05.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ffbeafbda15fcfcf98c3b7a62c77e05.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f61f5e704ccf72bfb570842a366f104.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f61f5e704ccf72bfb570842a366f104.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e119daabcfd640441083e17445834954.jpg\" _src=\"http://yanxuan.nosdn.127.net/e119daabcfd640441083e17445834954.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/010ba3b486af23613c04046c5829a7c2.jpg\" _src=\"http://yanxuan.nosdn.127.net/010ba3b486af23613c04046c5829a7c2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25f470d4479fbb74f9b6e105f8dedfbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/25f470d4479fbb74f9b6e105f8dedfbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e7c300089dba380e9f48d49ec964ff9.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e7c300089dba380e9f48d49ec964ff9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a7ab3c980cf291404489bd137efde6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a7ab3c980cf291404489bd137efde6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2fb08e93fa462fca26680a56737b9f91.jpg\" _src=\"http://yanxuan.nosdn.127.net/2fb08e93fa462fca26680a56737b9f91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0ad6f5f75871fa02408723457a8a8ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0ad6f5f75871fa02408723457a8a8ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3cecb48c44520393993ce5bc85da7ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3cecb48c44520393993ce5bc85da7ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cd68c353ca83624fa367f90592649b36.jpg\" _src=\"http://yanxuan.nosdn.127.net/cd68c353ca83624fa367f90592649b36.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9327cc921602b9d5b05147e4266910cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/9327cc921602b9d5b05147e4266910cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37cf3aa662187aa1126a5c41cb41d796.jpg\" _src=\"http://yanxuan.nosdn.127.net/37cf3aa662187aa1126a5c41cb41d796.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bef5ea165cda6dbbb109ea895b3f2fc5.jpg\" _src=\"http://yanxuan.nosdn.127.net/bef5ea165cda6dbbb109ea895b3f2fc5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/78c0d06130500a1247cb2a602264c61c.jpg\" _src=\"http://yanxuan.nosdn.127.net/78c0d06130500a1247cb2a602264c61c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79fd1cbd0c0d02ac58c2f449dcb6c97f.jpg\" _src=\"http://yanxuan.nosdn.127.net/79fd1cbd0c0d02ac58c2f449dcb6c97f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61acb2d95e1833aad988c183c94eebe2.jpg\" _src=\"http://yanxuan.nosdn.127.net/61acb2d95e1833aad988c183c94eebe2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7828935cd158c7bb6643186eb25be8bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/7828935cd158c7bb6643186eb25be8bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0409cef7649088f345fc64a348b49468.jpg\" _src=\"http://yanxuan.nosdn.127.net/0409cef7649088f345fc64a348b49468.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54e1beab4c0616b3147270201f978f2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/54e1beab4c0616b3147270201f978f2d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a75d34f45de74f2476f34ce329d57ff6.jpg\" _src=\"http://yanxuan.nosdn.127.net/a75d34f45de74f2476f34ce329d57ff6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/81607103dfd183acf7a364dd58e3cf93.jpg\" _src=\"http://yanxuan.nosdn.127.net/81607103dfd183acf7a364dd58e3cf93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/03cf20624d36fc793143ba7ba8b5c17f.jpg\" _src=\"http://yanxuan.nosdn.127.net/03cf20624d36fc793143ba7ba8b5c17f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da92a3b8729effd6f79e9c86b522f6ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/da92a3b8729effd6f79e9c86b522f6ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71aa5c2a762f4bced311f40323980552.jpg\" _src=\"http://yanxuan.nosdn.127.net/71aa5c2a762f4bced311f40323980552.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b81f52020b75b35b2254d327625713d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/b81f52020b75b35b2254d327625713d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f4d245eea01d80ce6769f308ccd7152.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f4d245eea01d80ce6769f308ccd7152.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c74f125472bf12a5b0ece0aaf15ef85.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c74f125472bf12a5b0ece0aaf15ef85.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6139fdd3fb21d66c527520a747a17fe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/6139fdd3fb21d66c527520a747a17fe3.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 9,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/09883bdbd9eec88ed615b99a275c0d54.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/87cf3a17ad40bfdcdc3314ea4591a5e8.png",
      "retail_price": 89,
      "sell_volume": 305,
      "primary_product_id": 1076004,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1072001,
      "category_id": 1008002,
      "goods_sn": "1072001",
      "name": "色织水洗棉绣花抱枕套",
      "brand_id": 1001020,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "清素色织，搭配水洗棉旧色的温柔",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/f8a74bd8e87987849bf2505c08ac69e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8a74bd8e87987849bf2505c08ac69e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be7ae107fc4b5085241507ed711254f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/be7ae107fc4b5085241507ed711254f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/143c402e82c2d99c3bc7cc51d064a62b.jpg\" _src=\"http://yanxuan.nosdn.127.net/143c402e82c2d99c3bc7cc51d064a62b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52f5b211f5da083da2bc9b5237c40b3b.jpg\" _src=\"http://yanxuan.nosdn.127.net/52f5b211f5da083da2bc9b5237c40b3b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5af00c6f7dc0d798dffe2cdc2da0f870.jpg\" _src=\"http://yanxuan.nosdn.127.net/5af00c6f7dc0d798dffe2cdc2da0f870.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/750bbc1c2207159b58a6de350060f5c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/750bbc1c2207159b58a6de350060f5c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d55dd54de50ff03b199261f3e021f388.jpg\" _src=\"http://yanxuan.nosdn.127.net/d55dd54de50ff03b199261f3e021f388.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b659703ddf8e35bb89ee5ff36e84b4f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/b659703ddf8e35bb89ee5ff36e84b4f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/573f30d45c3eea65f29a6497ac2b9a98.jpg\" _src=\"http://yanxuan.nosdn.127.net/573f30d45c3eea65f29a6497ac2b9a98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7d58eb147f2d8bedfc88ba08b544d7c.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7d58eb147f2d8bedfc88ba08b544d7c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec89200168dd4a703f7b89ec2be0b8a4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec89200168dd4a703f7b89ec2be0b8a4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d123c7d7b79ef8cd2703976e8bf1dbc.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d123c7d7b79ef8cd2703976e8bf1dbc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2797ba305c10b0e5fd6eafb384101402.jpg\" _src=\"http://yanxuan.nosdn.127.net/2797ba305c10b0e5fd6eafb384101402.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abcfbdafabe855e77598860b426fa5e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/abcfbdafabe855e77598860b426fa5e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d6ff672dae187d85d199ee1b1b62f9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d6ff672dae187d85d199ee1b1b62f9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e4424539e51dca9d000c6b67bea1f8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e4424539e51dca9d000c6b67bea1f8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/942da4a7c05d2a25be7a26decc40f53a.jpg\" _src=\"http://yanxuan.nosdn.127.net/942da4a7c05d2a25be7a26decc40f53a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c872c106b7da7d7b1167a9554c92aa1.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c872c106b7da7d7b1167a9554c92aa1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82607c78aedacd534a2e0f1b38e2e3e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/82607c78aedacd534a2e0f1b38e2e3e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/07e4e5ac1501706c8666eff4a703b5fb.jpg\" _src=\"http://yanxuan.nosdn.127.net/07e4e5ac1501706c8666eff4a703b5fb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a56805f63dfe98583e6b58eaa9dd595a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a56805f63dfe98583e6b58eaa9dd595a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ecdd28de374db2de0c0c2f0f50d0cd26.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecdd28de374db2de0c0c2f0f50d0cd26.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69fcb2566dea15f16a182b7e4e05893f.jpg\" _src=\"http://yanxuan.nosdn.127.net/69fcb2566dea15f16a182b7e4e05893f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bc3c5b3a6a14c8307e57842bf737601b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bc3c5b3a6a14c8307e57842bf737601b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d9c980cc924790bd7983bd80b0221a.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d9c980cc924790bd7983bd80b0221a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/787bdee826a5112c3e2bd4b9c15717e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/787bdee826a5112c3e2bd4b9c15717e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44dc985f99b3a95f255624a4d97857ca.jpg\" _src=\"http://yanxuan.nosdn.127.net/44dc985f99b3a95f255624a4d97857ca.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf117d9aef1ef7ab10d2ef040d9444c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf117d9aef1ef7ab10d2ef040d9444c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/07044f1a6c11d8d15e410a01482fb39a.jpg\" _src=\"http://yanxuan.nosdn.127.net/07044f1a6c11d8d15e410a01482fb39a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ca8ea48405cb43c901181a684c623dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ca8ea48405cb43c901181a684c623dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b4111628661d4216c8d0fc057e6d81e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b4111628661d4216c8d0fc057e6d81e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4adb10168dbfcee6f49460b2478de249.jpg\" _src=\"http://yanxuan.nosdn.127.net/4adb10168dbfcee6f49460b2478de249.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e798dd4abe3a833a4d0066453955ec1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/e798dd4abe3a833a4d0066453955ec1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/528abeae19cf1b5af2f49be4e142a2da.jpg\" _src=\"http://yanxuan.nosdn.127.net/528abeae19cf1b5af2f49be4e142a2da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2d3d5ae118bcacdfda08eb182a03c15a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2d3d5ae118bcacdfda08eb182a03c15a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3323a393743f839e12586418a0711123.jpg\" _src=\"http://yanxuan.nosdn.127.net/3323a393743f839e12586418a0711123.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ac29c5a1569d9fb37420f2eae835b91.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ac29c5a1569d9fb37420f2eae835b91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89ef4f7ec1c86f13d328c23c0429892a.jpg\" _src=\"http://yanxuan.nosdn.127.net/89ef4f7ec1c86f13d328c23c0429892a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b005b97dbffa333e49ff484abbcff04.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b005b97dbffa333e49ff484abbcff04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afa56b9370cdc27f27f8f951108cea4c.jpg\" _src=\"http://yanxuan.nosdn.127.net/afa56b9370cdc27f27f8f951108cea4c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5daae71eb699e7417e695472e1142678.jpg\" _src=\"http://yanxuan.nosdn.127.net/5daae71eb699e7417e695472e1142678.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3dbb71ba9fff82849a959deb8f5b7946.jpg\" _src=\"http://yanxuan.nosdn.127.net/3dbb71ba9fff82849a959deb8f5b7946.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e024ba974bad906db9e2a28d42293a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e024ba974bad906db9e2a28d42293a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/87e2d46daab9e1dd3e112c15692c66ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/87e2d46daab9e1dd3e112c15692c66ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/342bc9bb1cbf81d1bc7b33f77fa915ff.jpg\" _src=\"http://yanxuan.nosdn.127.net/342bc9bb1cbf81d1bc7b33f77fa915ff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f54d685cb3c111beff7ef58bb16252d6.jpg\" _src=\"http://yanxuan.nosdn.127.net/f54d685cb3c111beff7ef58bb16252d6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7c4c896daa0ac2ff5f89d5b738fc007.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7c4c896daa0ac2ff5f89d5b738fc007.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/839da4fb5874271d54f94c60ad4d7387.jpg\" _src=\"http://yanxuan.nosdn.127.net/839da4fb5874271d54f94c60ad4d7387.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7147d5acd91c330479762e51cf4257f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/7147d5acd91c330479762e51cf4257f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a9ca13fd9189e60df2f4a21783a3795.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a9ca13fd9189e60df2f4a21783a3795.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09fa8e6e95cc716138549e6b244a7924.jpg\" _src=\"http://yanxuan.nosdn.127.net/09fa8e6e95cc716138549e6b244a7924.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/772e18352ad2c156ee190f068726cd8c.jpg\" _src=\"http://yanxuan.nosdn.127.net/772e18352ad2c156ee190f068726cd8c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92c0a1e57d429d19fb7f4e678fa7fae1.jpg\" _src=\"http://yanxuan.nosdn.127.net/92c0a1e57d429d19fb7f4e678fa7fae1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88ddae38e8b363acdf79bfbe0547cc50.jpg\" _src=\"http://yanxuan.nosdn.127.net/88ddae38e8b363acdf79bfbe0547cc50.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c4c683112a57543d4e028754be53e0d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c4c683112a57543d4e028754be53e0d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f476dbaf8a8cae1e8a311edb77d4ea78.jpg\" _src=\"http://yanxuan.nosdn.127.net/f476dbaf8a8cae1e8a311edb77d4ea78.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7493e6d2980dc116654bdb3b24c1a3d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7493e6d2980dc116654bdb3b24c1a3d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/57e84b0e4b979782b0c3a4bce908d797.jpg\" _src=\"http://yanxuan.nosdn.127.net/57e84b0e4b979782b0c3a4bce908d797.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8eb47f38c324fd320c74bf0aa3ebdf1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8eb47f38c324fd320c74bf0aa3ebdf1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/622949bf7e667ea54eaf0861ac31c842.jpg\" _src=\"http://yanxuan.nosdn.127.net/622949bf7e667ea54eaf0861ac31c842.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 7,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a45cf27cc07e678cfe21257cb764711a.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/0e9d5954d7dc2477d9c46b730e05ab42.png",
      "retail_price": 49,
      "sell_volume": 121,
      "primary_product_id": 1076007,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1081000,
      "category_id": 1008002,
      "goods_sn": "1081000",
      "name": "北欧风珊瑚绒多功能暖手枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "手枕坐垫两用",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/19ce01a5361a70388e7d40e94ccd3495.jpg\" _src=\"http://yanxuan.nosdn.127.net/19ce01a5361a70388e7d40e94ccd3495.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a037a815a9c11449de1c5c94d6a6d987.jpg\" _src=\"http://yanxuan.nosdn.127.net/a037a815a9c11449de1c5c94d6a6d987.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7ccc425d60247f8468ede401cb74683.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7ccc425d60247f8468ede401cb74683.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/039951ed06296e8065f7b219a4a111de.jpg\" _src=\"http://yanxuan.nosdn.127.net/039951ed06296e8065f7b219a4a111de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37576f4179798648632a694da355996f.jpg\" _src=\"http://yanxuan.nosdn.127.net/37576f4179798648632a694da355996f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d45db0fcfff3fb9ced3f6bc5e5d6a23.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d45db0fcfff3fb9ced3f6bc5e5d6a23.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e46450a60e9bc60bca3f483ad14337b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/e46450a60e9bc60bca3f483ad14337b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/071c557f2845aa18a7f4d80f556b1178.jpg\" _src=\"http://yanxuan.nosdn.127.net/071c557f2845aa18a7f4d80f556b1178.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5935e928d9b1b6781db188cf41f93424.jpg\" _src=\"http://yanxuan.nosdn.127.net/5935e928d9b1b6781db188cf41f93424.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83f8bac183a90e5d8f32c698813ef046.jpg\" _src=\"http://yanxuan.nosdn.127.net/83f8bac183a90e5d8f32c698813ef046.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7ae7816d84e084b9df010ae92f7c0bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7ae7816d84e084b9df010ae92f7c0bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c89f0917bceb94f0e300df77d08c75e.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c89f0917bceb94f0e300df77d08c75e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62c52e788f028eab5b4927671f4aa109.jpg\" _src=\"http://yanxuan.nosdn.127.net/62c52e788f028eab5b4927671f4aa109.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93b9efc4c1b39c065c0dde2974a9dc52.jpg\" _src=\"http://yanxuan.nosdn.127.net/93b9efc4c1b39c065c0dde2974a9dc52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40da45628d48712880dc64843aba8e6a.jpg\" _src=\"http://yanxuan.nosdn.127.net/40da45628d48712880dc64843aba8e6a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec12badecafb5dd8f67b52efa6cf4b15.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec12badecafb5dd8f67b52efa6cf4b15.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bde2888497b52e724ca72d42a86578d1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bde2888497b52e724ca72d42a86578d1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f1b163294dff20ac85a5f6dc8016500.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f1b163294dff20ac85a5f6dc8016500.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2f970069e7d381421dec8c407fcd2a7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2f970069e7d381421dec8c407fcd2a7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b852d0821395488c729a4d09941b2ea7.jpg\" _src=\"http://yanxuan.nosdn.127.net/b852d0821395488c729a4d09941b2ea7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/660168255d39ded4c1d2038cff5d253f.jpg\" _src=\"http://yanxuan.nosdn.127.net/660168255d39ded4c1d2038cff5d253f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7fe09efd35ef54dfa0a92c8059971995.jpg\" _src=\"http://yanxuan.nosdn.127.net/7fe09efd35ef54dfa0a92c8059971995.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f13328e747638a9681502f97d0fc032a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f13328e747638a9681502f97d0fc032a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/05c538811b7d8d37b15e9b168b45ed19.jpg\" _src=\"http://yanxuan.nosdn.127.net/05c538811b7d8d37b15e9b168b45ed19.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e597815f2bbf76f2c078326d3cd255e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/e597815f2bbf76f2c078326d3cd255e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/73d7bd31e90a2bdc79263dde20e2496c.jpg\" _src=\"http://yanxuan.nosdn.127.net/73d7bd31e90a2bdc79263dde20e2496c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e10091f21b56c616ac4ab51decab76a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e10091f21b56c616ac4ab51decab76a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5023b92342a2f936996c2eaf2e79f1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5023b92342a2f936996c2eaf2e79f1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a090e4b9269a901e660cc35a1c38975a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a090e4b9269a901e660cc35a1c38975a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85c707ebaae017ab65bf5e2266ec7c6d.jpg\" _src=\"http://yanxuan.nosdn.127.net/85c707ebaae017ab65bf5e2266ec7c6d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/30a57bf64ad98af99955d90e45ae9f3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/30a57bf64ad98af99955d90e45ae9f3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ec59f055c27c776ee5ec635e1e64b79.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ec59f055c27c776ee5ec635e1e64b79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f39b93929486b2ba679ed22fac5021b6.jpg\" _src=\"http://yanxuan.nosdn.127.net/f39b93929486b2ba679ed22fac5021b6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ea9e76b9b0988c823796752cd3bc4e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ea9e76b9b0988c823796752cd3bc4e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b952cc40eab4b590943ad91fb35c4ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b952cc40eab4b590943ad91fb35c4ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5f5e5f1d2adbb2aaaf10e1e38913206b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5f5e5f1d2adbb2aaaf10e1e38913206b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50c14625bb7a2d0331fee4181ae22455.jpg\" _src=\"http://yanxuan.nosdn.127.net/50c14625bb7a2d0331fee4181ae22455.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7af5402277f0cfd4e9ac2bf9c0c0cd8e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7af5402277f0cfd4e9ac2bf9c0c0cd8e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b413e4e18e70b2b1bddb54358fbf507e.jpg\" _src=\"http://yanxuan.nosdn.127.net/b413e4e18e70b2b1bddb54358fbf507e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2006d2a3ff91300d1265ce875433484a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2006d2a3ff91300d1265ce875433484a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35c5c281c7b8bfe5a67704abfbd0f550.jpg\" _src=\"http://yanxuan.nosdn.127.net/35c5c281c7b8bfe5a67704abfbd0f550.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f30d0dd64c48d72f543cf7f48f66f48.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f30d0dd64c48d72f543cf7f48f66f48.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/13632b105431e683733b69d8a065d458.jpg\" _src=\"http://yanxuan.nosdn.127.net/13632b105431e683733b69d8a065d458.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3a10c77b61704c1efa426d566ead340.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3a10c77b61704c1efa426d566ead340.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 22,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/eb9fd89dcabcbcf7ed7b86a3cb47c96e.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/cc45baafad00405699552c187c64c512.png",
      "retail_price": 49,
      "sell_volume": 997,
      "primary_product_id": 1085010,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1081002,
      "category_id": 1008002,
      "goods_sn": "1081002",
      "name": "北欧风珊瑚绒多功能抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "靠枕暖手毛毯多用",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/d3afdc4dc4f7e8700abd3befd8786f9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3afdc4dc4f7e8700abd3befd8786f9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/690e4238d3c6fe734e5a5a8e5d567cf2.jpg\" _src=\"http://yanxuan.nosdn.127.net/690e4238d3c6fe734e5a5a8e5d567cf2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3bb465550fcf6bafcde2b11b4a96d799.jpg\" _src=\"http://yanxuan.nosdn.127.net/3bb465550fcf6bafcde2b11b4a96d799.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b4ba8661f77ff02edc7a172ea1489a3.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b4ba8661f77ff02edc7a172ea1489a3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ededcff020a14eecad669b5beeba3f30.jpg\" _src=\"http://yanxuan.nosdn.127.net/ededcff020a14eecad669b5beeba3f30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/394992289ec493441e7e91dd8a6e856b.jpg\" _src=\"http://yanxuan.nosdn.127.net/394992289ec493441e7e91dd8a6e856b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f06eb02e8ed368a868dfd8137d1c7f3b.jpg\" _src=\"http://yanxuan.nosdn.127.net/f06eb02e8ed368a868dfd8137d1c7f3b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cec7fcfda67bf3ed1ee66e887614d633.jpg\" _src=\"http://yanxuan.nosdn.127.net/cec7fcfda67bf3ed1ee66e887614d633.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19ffcfd2a998820e92656611ba6ccd99.jpg\" _src=\"http://yanxuan.nosdn.127.net/19ffcfd2a998820e92656611ba6ccd99.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c698e643a9ababb498f36b2dd948f59.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c698e643a9ababb498f36b2dd948f59.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9746e6314f6aec06be56e6b1f54972c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9746e6314f6aec06be56e6b1f54972c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/769eee41f1452888fa632c07551ca400.jpg\" _src=\"http://yanxuan.nosdn.127.net/769eee41f1452888fa632c07551ca400.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65c740031e1cd5792aecc6333710fe06.jpg\" _src=\"http://yanxuan.nosdn.127.net/65c740031e1cd5792aecc6333710fe06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/42361e27db7a3b76705568c0f57bfd43.jpg\" _src=\"http://yanxuan.nosdn.127.net/42361e27db7a3b76705568c0f57bfd43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8a3048b4a8ea13487faa1ff51c394ad3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8a3048b4a8ea13487faa1ff51c394ad3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/032041aaae3d703194d7fab7599c4495.jpg\" _src=\"http://yanxuan.nosdn.127.net/032041aaae3d703194d7fab7599c4495.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2478a21152ad10d517af58aaaed64214.jpg\" _src=\"http://yanxuan.nosdn.127.net/2478a21152ad10d517af58aaaed64214.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92691014c72fd7f34f6fada58162011f.jpg\" _src=\"http://yanxuan.nosdn.127.net/92691014c72fd7f34f6fada58162011f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9dc547b23d58f4a835008b55f797f4bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/9dc547b23d58f4a835008b55f797f4bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf6a80f009ba96e51851dce228e542b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf6a80f009ba96e51851dce228e542b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52674285cdb5d2ea19967d3188d1ff8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/52674285cdb5d2ea19967d3188d1ff8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eeb3c5128f915416f4b60a968230d320.jpg\" _src=\"http://yanxuan.nosdn.127.net/eeb3c5128f915416f4b60a968230d320.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/998cc7acd5ce1797aa4b32f8ef775148.jpg\" _src=\"http://yanxuan.nosdn.127.net/998cc7acd5ce1797aa4b32f8ef775148.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d7d12038de9483c3974c3ad8f20927a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/d7d12038de9483c3974c3ad8f20927a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f3c6b9f3fdf0c48156251636e513720e.jpg\" _src=\"http://yanxuan.nosdn.127.net/f3c6b9f3fdf0c48156251636e513720e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/367b80cefe0803348720f82f1c30cfe7.jpg\" _src=\"http://yanxuan.nosdn.127.net/367b80cefe0803348720f82f1c30cfe7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c360e0a65e58cc1c04e01eed6f04b54b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c360e0a65e58cc1c04e01eed6f04b54b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6e60d12aff676400bad21d0c93b67803.jpg\" _src=\"http://yanxuan.nosdn.127.net/6e60d12aff676400bad21d0c93b67803.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8be1fb462d145316ec2264d5025b8a48.jpg\" _src=\"http://yanxuan.nosdn.127.net/8be1fb462d145316ec2264d5025b8a48.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80725f3251d122a8bc66b20814648310.jpg\" _src=\"http://yanxuan.nosdn.127.net/80725f3251d122a8bc66b20814648310.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a6a82ed8c28b0c60b45bb38e4e7ce04.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a6a82ed8c28b0c60b45bb38e4e7ce04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae881c80e00c34e59c7fd77f829b9931.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae881c80e00c34e59c7fd77f829b9931.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10d7b57b8772053d38fca8e7f6856bac.jpg\" _src=\"http://yanxuan.nosdn.127.net/10d7b57b8772053d38fca8e7f6856bac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6d43e30b2aaac4a81dec473fc2842984.jpg\" _src=\"http://yanxuan.nosdn.127.net/6d43e30b2aaac4a81dec473fc2842984.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdd8426becc5a730730838e264c8c998.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdd8426becc5a730730838e264c8c998.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2aaf853063048b8485c1219b8ba55ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2aaf853063048b8485c1219b8ba55ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70604ff736ccc200037d247a274ac128.jpg\" _src=\"http://yanxuan.nosdn.127.net/70604ff736ccc200037d247a274ac128.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3778c8814cba4fa56d697d6e7c84e5dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/3778c8814cba4fa56d697d6e7c84e5dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa66cda001dd6ba7281f9808da9a344b.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa66cda001dd6ba7281f9808da9a344b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65955a09afe2dfa08a92e3b70bda0f5d.jpg\" _src=\"http://yanxuan.nosdn.127.net/65955a09afe2dfa08a92e3b70bda0f5d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/46bd1859ec91d296d8367e2e6a97ec11.jpg\" _src=\"http://yanxuan.nosdn.127.net/46bd1859ec91d296d8367e2e6a97ec11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33259dcc01613bbf0bb8313f9129e7bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/33259dcc01613bbf0bb8313f9129e7bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5fa03cc2c17cc38da8dc84d0c0e42fa2.jpg\" _src=\"http://yanxuan.nosdn.127.net/5fa03cc2c17cc38da8dc84d0c0e42fa2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5baa2bc5c725dd3d8522b7766830bcb.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5baa2bc5c725dd3d8522b7766830bcb.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 21,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/b87b4b80910fa03b92923997fd4aabd9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/380cfcd5d8bc22360de089f0b4eb11da.png",
      "retail_price": 89,
      "sell_volume": 132,
      "primary_product_id": 1085012,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 1
    },
    {
      "id": 1115052,
      "category_id": 1008002,
      "goods_sn": "1115052",
      "name": "日式和风蔺草蒲团坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "龙眉蔺草编织 日式茶禅风",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/c5c39ed4982045a32efde6f8e4b3d327.jpg\" _src=\"http://yanxuan.nosdn.127.net/c5c39ed4982045a32efde6f8e4b3d327.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/385b1a317b993c403f5b1532bf714592.jpg\" _src=\"http://yanxuan.nosdn.127.net/385b1a317b993c403f5b1532bf714592.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97c44d5c2411a2b8bb39ee34957783bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/97c44d5c2411a2b8bb39ee34957783bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/489a326e13a5bb3ce44a40fc71ccbc40.jpg\" _src=\"http://yanxuan.nosdn.127.net/489a326e13a5bb3ce44a40fc71ccbc40.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2d6eb8e6ba1de0db4bdc1d4ef8d124d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2d6eb8e6ba1de0db4bdc1d4ef8d124d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e723ef50260b98666955796f6dab4c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e723ef50260b98666955796f6dab4c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3cd9585a68c6b746f509408c2c16783a.jpg\" _src=\"http://yanxuan.nosdn.127.net/3cd9585a68c6b746f509408c2c16783a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/582bdb6e01ad3b8f2d76d0124dfdcf8e.jpg\" _src=\"http://yanxuan.nosdn.127.net/582bdb6e01ad3b8f2d76d0124dfdcf8e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8dd281a87afd1ae88dc05e1db35142a4.jpg\" _src=\"http://yanxuan.nosdn.127.net/8dd281a87afd1ae88dc05e1db35142a4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/73a608d337ac09b75b4bd14d8170b6d6.jpg\" _src=\"http://yanxuan.nosdn.127.net/73a608d337ac09b75b4bd14d8170b6d6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fdc10bae153b0dda81dd53b57c2b9e10.jpg\" _src=\"http://yanxuan.nosdn.127.net/fdc10bae153b0dda81dd53b57c2b9e10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cccdb8b1831f0b70306a4b4eed8859db.jpg\" _src=\"http://yanxuan.nosdn.127.net/cccdb8b1831f0b70306a4b4eed8859db.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5baf78b4175b0fdb0132b5d83bb7e279.jpg\" _src=\"http://yanxuan.nosdn.127.net/5baf78b4175b0fdb0132b5d83bb7e279.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e613832e2b3e0cfcad1c42e6cf3d6d3e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e613832e2b3e0cfcad1c42e6cf3d6d3e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de9c7cedfd555ceb5adfed1c0c96b9b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/de9c7cedfd555ceb5adfed1c0c96b9b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61a0ecae290671c15ac857e0f5b8fb5f.jpg\" _src=\"http://yanxuan.nosdn.127.net/61a0ecae290671c15ac857e0f5b8fb5f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8f15359576d133d55457f69c05aeab8.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8f15359576d133d55457f69c05aeab8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aae2ff89028e265b06656aa63a94c58e.jpg\" _src=\"http://yanxuan.nosdn.127.net/aae2ff89028e265b06656aa63a94c58e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbecb94e2a020007505cad42c4e8553a.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbecb94e2a020007505cad42c4e8553a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4adb8529010d4348b90cdc445f37d241.jpg\" _src=\"http://yanxuan.nosdn.127.net/4adb8529010d4348b90cdc445f37d241.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/953207acdb90210c681deb18b59fdadb.jpg\" _src=\"http://yanxuan.nosdn.127.net/953207acdb90210c681deb18b59fdadb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa5b73dea7f39614c01de4ee8acdc216.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa5b73dea7f39614c01de4ee8acdc216.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2b7ccd3a548618f2fadb20aee9ab9531.jpg\" _src=\"http://yanxuan.nosdn.127.net/2b7ccd3a548618f2fadb20aee9ab9531.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ecde950588789c70df2222f1ded0f579.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecde950588789c70df2222f1ded0f579.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/597505ee5976bf7f68646ef2321c5b39.jpg\" _src=\"http://yanxuan.nosdn.127.net/597505ee5976bf7f68646ef2321c5b39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f317d788383403a224a191452183b9f.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f317d788383403a224a191452183b9f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ca568894e24f4aa5d6eaf4174667ffa.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ca568894e24f4aa5d6eaf4174667ffa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdbf86365486d602bc2c2b1aa4bd8781.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdbf86365486d602bc2c2b1aa4bd8781.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa9db3d211c93fa9d2914754464e679c.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa9db3d211c93fa9d2914754464e679c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/58e5cd852682d404200f57471e883485.jpg\" _src=\"http://yanxuan.nosdn.127.net/58e5cd852682d404200f57471e883485.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14cc6189a160dcf8f0d2f0d0bd0b7f27.jpg\" _src=\"http://yanxuan.nosdn.127.net/14cc6189a160dcf8f0d2f0d0bd0b7f27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c49b33afea38804de07fc9a6bb80dda9.jpg\" _src=\"http://yanxuan.nosdn.127.net/c49b33afea38804de07fc9a6bb80dda9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8cf4bc3c1b476cba2ec6290b02c698be.jpg\" _src=\"http://yanxuan.nosdn.127.net/8cf4bc3c1b476cba2ec6290b02c698be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3d5eb1291c79204e2e23dede15b8cac.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3d5eb1291c79204e2e23dede15b8cac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38791f147ef4ee52bfee5e240f2a5f52.jpg\" _src=\"http://yanxuan.nosdn.127.net/38791f147ef4ee52bfee5e240f2a5f52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9756648996576857cabe3740da2edaa6.jpg\" _src=\"http://yanxuan.nosdn.127.net/9756648996576857cabe3740da2edaa6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f4247a5ccb0f39be52a8c99cb15f92f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/f4247a5ccb0f39be52a8c99cb15f92f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40d0ceae7b2300246501b72540727505.jpg\" _src=\"http://yanxuan.nosdn.127.net/40d0ceae7b2300246501b72540727505.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/14603e5d6e54d7e1abaae04ea713de08.jpg\" _src=\"http://yanxuan.nosdn.127.net/14603e5d6e54d7e1abaae04ea713de08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/06d66618b49e447645e3650dc6cb11ca.jpg\" _src=\"http://yanxuan.nosdn.127.net/06d66618b49e447645e3650dc6cb11ca.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ef12ad1adb0d16743a0054489846a13.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ef12ad1adb0d16743a0054489846a13.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99d648a6665d2a25f790a469c464d34b.jpg\" _src=\"http://yanxuan.nosdn.127.net/99d648a6665d2a25f790a469c464d34b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76e121103fb90fdf267eb204af59c0d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/76e121103fb90fdf267eb204af59c0d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9d92a1874c26534262643772dbdef1d2.jpg\" _src=\"http://yanxuan.nosdn.127.net/9d92a1874c26534262643772dbdef1d2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cb04ad36ddc0b45066f8233ab9cf888.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cb04ad36ddc0b45066f8233ab9cf888.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cdb4947e9c035fea2bb271c9f0b43d2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/cdb4947e9c035fea2bb271c9f0b43d2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55c1446b40d52e2da86f92fccc47ea2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/55c1446b40d52e2da86f92fccc47ea2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/339c0d5acef5c3029fd3c0d500883ce5.jpg\" _src=\"http://yanxuan.nosdn.127.net/339c0d5acef5c3029fd3c0d500883ce5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11dc59302185026721eaa23509c333ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/11dc59302185026721eaa23509c333ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/81ed48a7099d3bfa9860fcdd4e546b60.jpg\" _src=\"http://yanxuan.nosdn.127.net/81ed48a7099d3bfa9860fcdd4e546b60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c615061f6c675ba67897e03e1f9cee17.jpg\" _src=\"http://yanxuan.nosdn.127.net/c615061f6c675ba67897e03e1f9cee17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e30a5c3df143363971c97e75f254818d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e30a5c3df143363971c97e75f254818d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b33a8b54250cf02206d1d9fa5674725.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b33a8b54250cf02206d1d9fa5674725.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf292ce53420b314368494c36b189ce1.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf292ce53420b314368494c36b189ce1.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 18,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/66d736aa8e3e33e3c76a014e1379c9a9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/39dea35a3ea2361e4b054ee2f421af53.png",
      "retail_price": 86,
      "sell_volume": 5586,
      "primary_product_id": 1116105,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1128002,
      "category_id": 1008002,
      "goods_sn": "1128002",
      "name": "清新趣粉系列居家地毯 青粉拼接",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "清新撞色 细腻柔软",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/191b701367615b452976b4c740ef1c52.jpg\" _src=\"http://yanxuan.nosdn.127.net/191b701367615b452976b4c740ef1c52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f83f2a2b556d9d0b4b4a65ca76f4689.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f83f2a2b556d9d0b4b4a65ca76f4689.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/119231f5f75494b2249cd14009b452aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/119231f5f75494b2249cd14009b452aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/085c0b2b140f9b3e499209f3ca2b3b16.jpg\" _src=\"http://yanxuan.nosdn.127.net/085c0b2b140f9b3e499209f3ca2b3b16.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ac2cdba24df037dfe0704bd47c73d3e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/ac2cdba24df037dfe0704bd47c73d3e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35def50dabd355332d47a994e29a53c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/35def50dabd355332d47a994e29a53c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0378678601a27aa2e0fea8fcd757ae51.jpg\" _src=\"http://yanxuan.nosdn.127.net/0378678601a27aa2e0fea8fcd757ae51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c3d214fea7c5a768c7a0f77172a70d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c3d214fea7c5a768c7a0f77172a70d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bec41337e525e74998290e7378f3bb8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bec41337e525e74998290e7378f3bb8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d5d50c46c26a0c2be14d2c845a4e15c5.jpg\" _src=\"http://yanxuan.nosdn.127.net/d5d50c46c26a0c2be14d2c845a4e15c5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c138155947879f4af0e7ce3c7d4713d.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c138155947879f4af0e7ce3c7d4713d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da7c0824e22218d320719560989d537e.jpg\" _src=\"http://yanxuan.nosdn.127.net/da7c0824e22218d320719560989d537e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bf35a5b2a1747108cb8d225f0da227d.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bf35a5b2a1747108cb8d225f0da227d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e93c3ee67c2f953fae54295b0f4a7173.jpg\" _src=\"http://yanxuan.nosdn.127.net/e93c3ee67c2f953fae54295b0f4a7173.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa47796942f2ba1f6bf0032fe316ac27.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa47796942f2ba1f6bf0032fe316ac27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f116e257387af4f48bf2ddb8c840132.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f116e257387af4f48bf2ddb8c840132.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a756a78742cd1e018a66e40e0cf3f5ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/a756a78742cd1e018a66e40e0cf3f5ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/567a0391d29b41c75216203f0327360d.jpg\" _src=\"http://yanxuan.nosdn.127.net/567a0391d29b41c75216203f0327360d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e3bb469a99952ad770a1782ebabe0a3.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e3bb469a99952ad770a1782ebabe0a3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/98e4edc31d260fcfdff9d74527a36361.jpg\" _src=\"http://yanxuan.nosdn.127.net/98e4edc31d260fcfdff9d74527a36361.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8f9871f90756a1833bea06961285087.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8f9871f90756a1833bea06961285087.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa9d442de4aa9b93b48fefafe0f869b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa9d442de4aa9b93b48fefafe0f869b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8c3c00ea6a2f13c5ce37b6dec024edf5.jpg\" _src=\"http://yanxuan.nosdn.127.net/8c3c00ea6a2f13c5ce37b6dec024edf5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d83a1dc525bb6aa23d456efd5a2c74c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d83a1dc525bb6aa23d456efd5a2c74c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7397347cfc3d7ce697386941201d1615.jpg\" _src=\"http://yanxuan.nosdn.127.net/7397347cfc3d7ce697386941201d1615.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e40e07ef01e1950ddb708d6ed56eea3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e40e07ef01e1950ddb708d6ed56eea3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb59b7f4df5d97e9ac407fe75e095e81.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb59b7f4df5d97e9ac407fe75e095e81.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6660e07c91870230941f9bfe160f9f49.jpg\" _src=\"http://yanxuan.nosdn.127.net/6660e07c91870230941f9bfe160f9f49.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e40bb0099d592ca0f1335eabe43570cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/e40bb0099d592ca0f1335eabe43570cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7310efd4551e1a851668d01733711d39.jpg\" _src=\"http://yanxuan.nosdn.127.net/7310efd4551e1a851668d01733711d39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4c7ab57bdf16a7a88e526e82deba2879.jpg\" _src=\"http://yanxuan.nosdn.127.net/4c7ab57bdf16a7a88e526e82deba2879.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e1a120dc4898e9e871d4005d30c7937.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e1a120dc4898e9e871d4005d30c7937.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22fe678cf2b8e594c15fba60f86b717e.jpg\" _src=\"http://yanxuan.nosdn.127.net/22fe678cf2b8e594c15fba60f86b717e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c7e4053e6340d8fc377babc65cd40823.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7e4053e6340d8fc377babc65cd40823.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ae576390b96e274b10c71104e210d33.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ae576390b96e274b10c71104e210d33.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/425feec1ad943958c28edaf1504af645.jpg\" _src=\"http://yanxuan.nosdn.127.net/425feec1ad943958c28edaf1504af645.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e8d1bd0e0277e74509d074f2a931f1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e8d1bd0e0277e74509d074f2a931f1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e67f6b3d18df8ddf931b4468f35d4fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e67f6b3d18df8ddf931b4468f35d4fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33951c6621e5b91ee1c1b9958f9bb57a.jpg\" _src=\"http://yanxuan.nosdn.127.net/33951c6621e5b91ee1c1b9958f9bb57a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e80772f6663a57de51494fec4369524b.jpg\" _src=\"http://yanxuan.nosdn.127.net/e80772f6663a57de51494fec4369524b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e2516cafe760408782a8427a5015b98.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e2516cafe760408782a8427a5015b98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2fe4275c5b83193c1562e2f5dbf72442.jpg\" _src=\"http://yanxuan.nosdn.127.net/2fe4275c5b83193c1562e2f5dbf72442.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1d4aa2f956ef90e826b50cb16db731a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1d4aa2f956ef90e826b50cb16db731a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c9afc1b180779690891a23e9adb2265.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c9afc1b180779690891a23e9adb2265.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d4323b01083e2aa3eec9e28402b612b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d4323b01083e2aa3eec9e28402b612b.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 27,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/dbf282e81ab8b0dbc4b4ad1f4fd6d1e3.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/a1094a808ffb3a52a6cb13565a283d98.png",
      "retail_price": 599,
      "sell_volume": 137,
      "primary_product_id": 1128017,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1130037,
      "category_id": 1008002,
      "goods_sn": "1130037",
      "name": "帆布丝羽绒多用坐垫",
      "brand_id": 1001000,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "柔软蓬松，透气防螨。",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/96eb609f4f459ab9c502eca7d6e7e204.jpg\" _src=\"http://yanxuan.nosdn.127.net/96eb609f4f459ab9c502eca7d6e7e204.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a86dcf95f3a56db6b7f99f35585dbf2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a86dcf95f3a56db6b7f99f35585dbf2d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bced9d39bcb740a4655ce725f4823e96.jpg\" _src=\"http://yanxuan.nosdn.127.net/bced9d39bcb740a4655ce725f4823e96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11213e448a23292458adc934a643c076.jpg\" _src=\"http://yanxuan.nosdn.127.net/11213e448a23292458adc934a643c076.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9116d858fd59f1ed32fc8a692dfc3fed.jpg\" _src=\"http://yanxuan.nosdn.127.net/9116d858fd59f1ed32fc8a692dfc3fed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b5982e9a43ccaa724f397c9e777b026.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b5982e9a43ccaa724f397c9e777b026.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e4397bee1cf9589eaaf06b8fe9d0a778.jpg\" _src=\"http://yanxuan.nosdn.127.net/e4397bee1cf9589eaaf06b8fe9d0a778.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/740affd3cef0ef40378c2cb265322f15.jpg\" _src=\"http://yanxuan.nosdn.127.net/740affd3cef0ef40378c2cb265322f15.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6aeacc205ef12e2a475eb7a8e8d1eedc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6aeacc205ef12e2a475eb7a8e8d1eedc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/119709a17d08f2c1c48d95d24b34ca3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/119709a17d08f2c1c48d95d24b34ca3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8332210d4b81d04f42612fc097db259a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8332210d4b81d04f42612fc097db259a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be1775926acb0e26b6012cba7893e979.jpg\" _src=\"http://yanxuan.nosdn.127.net/be1775926acb0e26b6012cba7893e979.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c6463b2f53c89273f1f79b22dd9e399.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c6463b2f53c89273f1f79b22dd9e399.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38ad3258ebf23df5164854fe403d1ecf.jpg\" _src=\"http://yanxuan.nosdn.127.net/38ad3258ebf23df5164854fe403d1ecf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dc5f238dcb73c249f813233d81156c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dc5f238dcb73c249f813233d81156c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb132e2e8a254b8cbc345900f6fe3c39.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb132e2e8a254b8cbc345900f6fe3c39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0603f40fefd14ee24e83102c5f09100a.jpg\" _src=\"http://yanxuan.nosdn.127.net/0603f40fefd14ee24e83102c5f09100a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/45966f38135adc1280a667040d8e02c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/45966f38135adc1280a667040d8e02c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1064a54404b6c795eae261334697e050.jpg\" _src=\"http://yanxuan.nosdn.127.net/1064a54404b6c795eae261334697e050.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ef89417a81ac1893c95179585bf1140.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ef89417a81ac1893c95179585bf1140.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c2cd2da4d75a63ada7c655e53c223a0e.jpg\" _src=\"http://yanxuan.nosdn.127.net/c2cd2da4d75a63ada7c655e53c223a0e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e942519448a5de394885730e0e3e4694.jpg\" _src=\"http://yanxuan.nosdn.127.net/e942519448a5de394885730e0e3e4694.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d016a18c381916813c2eaf46c3f791c1.jpg\" _src=\"http://yanxuan.nosdn.127.net/d016a18c381916813c2eaf46c3f791c1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6935f94bc80c11c89c3f8a2aa02c4273.jpg\" _src=\"http://yanxuan.nosdn.127.net/6935f94bc80c11c89c3f8a2aa02c4273.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9dedb80199b09770b98fa46cd8a8752d.jpg\" _src=\"http://yanxuan.nosdn.127.net/9dedb80199b09770b98fa46cd8a8752d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f447537304e43a44b1e75272d3334899.jpg\" _src=\"http://yanxuan.nosdn.127.net/f447537304e43a44b1e75272d3334899.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10d901511a3d5f03be68bd64dbadfe1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/10d901511a3d5f03be68bd64dbadfe1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b03a90f7bb697a9bc6e0be9d9997b11.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b03a90f7bb697a9bc6e0be9d9997b11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/62b277f50e7cca075cd2565a4f2b4466.jpg\" _src=\"http://yanxuan.nosdn.127.net/62b277f50e7cca075cd2565a4f2b4466.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e304f8f1ea10792be9072d3c7a4a8359.jpg\" _src=\"http://yanxuan.nosdn.127.net/e304f8f1ea10792be9072d3c7a4a8359.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5d7c39350bee7fdc8bdb78a27eb83a17.jpg\" _src=\"http://yanxuan.nosdn.127.net/5d7c39350bee7fdc8bdb78a27eb83a17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/742927f31cadc641a7b9bb3fc5eebfe3.jpg\" _src=\"http://yanxuan.nosdn.127.net/742927f31cadc641a7b9bb3fc5eebfe3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2562d7d1a0fa4b9497e4ec719f08a8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2562d7d1a0fa4b9497e4ec719f08a8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/430442f4524e66347fbbf10aaf213a07.jpg\" _src=\"http://yanxuan.nosdn.127.net/430442f4524e66347fbbf10aaf213a07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/620ec1f6387fa84f5518ad2484ebaa91.jpg\" _src=\"http://yanxuan.nosdn.127.net/620ec1f6387fa84f5518ad2484ebaa91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/455f215b9a402ed9c0c0972c0abddbb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/455f215b9a402ed9c0c0972c0abddbb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1def5c3403bdf5cd7e11b85354542452.jpg\" _src=\"http://yanxuan.nosdn.127.net/1def5c3403bdf5cd7e11b85354542452.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97348238ae3c27a56ff46e1b6c3deb3b.jpg\" _src=\"http://yanxuan.nosdn.127.net/97348238ae3c27a56ff46e1b6c3deb3b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3739461a5eb338a70e7d34a86ff26d1a.jpg\" _src=\"http://yanxuan.nosdn.127.net/3739461a5eb338a70e7d34a86ff26d1a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/96fae2f2cc374d459c3969e7a7cc1a83.jpg\" _src=\"http://yanxuan.nosdn.127.net/96fae2f2cc374d459c3969e7a7cc1a83.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c1654fc509c8c77e9fe4c75ffc099f24.jpg\" _src=\"http://yanxuan.nosdn.127.net/c1654fc509c8c77e9fe4c75ffc099f24.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf95ab8945e61c7180eba1e01721b15a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf95ab8945e61c7180eba1e01721b15a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b054e088382a0cb32a529082c52745e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/b054e088382a0cb32a529082c52745e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53d517d1ca7532cde5cc74ad2a10dc17.jpg\" _src=\"http://yanxuan.nosdn.127.net/53d517d1ca7532cde5cc74ad2a10dc17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6222e1fd9b42422e8454cc087a0e0358.jpg\" _src=\"http://yanxuan.nosdn.127.net/6222e1fd9b42422e8454cc087a0e0358.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8995022af1826e846b7a143e7b8b325.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8995022af1826e846b7a143e7b8b325.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a12c940956234db2f60a2b5b51d6a35.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a12c940956234db2f60a2b5b51d6a35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4be7d3058e6eec27a4be033642359535.jpg\" _src=\"http://yanxuan.nosdn.127.net/4be7d3058e6eec27a4be033642359535.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2eca2f02d4ec269cc1893876fb17511a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2eca2f02d4ec269cc1893876fb17511a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf761716e3b430f63e059a891703200e.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf761716e3b430f63e059a891703200e.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 17,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2d1f51656c0bff4989e43b17b42f7ad9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/19ecd7c6f6f31219cf75117238d95139.png",
      "retail_price": 39,
      "sell_volume": 9661,
      "primary_product_id": 1130120,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1130041,
      "category_id": 1008002,
      "goods_sn": "1130041",
      "name": "皮毛一体多用长毛坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "澳洲羊毛的细腻触感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/a83b7218bebd4a83c0b9f6f8a5ea6d08.jpg\" _src=\"http://yanxuan.nosdn.127.net/a83b7218bebd4a83c0b9f6f8a5ea6d08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7eb4d058e83cd9b6aadf5c20c63bcb1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7eb4d058e83cd9b6aadf5c20c63bcb1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/731f44716c3c585f563196c887544f52.jpg\" _src=\"http://yanxuan.nosdn.127.net/731f44716c3c585f563196c887544f52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59afb77cc310a6fde3eabd6401e8bab1.jpg\" _src=\"http://yanxuan.nosdn.127.net/59afb77cc310a6fde3eabd6401e8bab1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db3c78a5adad2a0ea8d219083e8547b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/db3c78a5adad2a0ea8d219083e8547b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/267cc4ac41d6632aec5b18e2026739dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/267cc4ac41d6632aec5b18e2026739dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76a367af57d38c0bc77086e784c2b1d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/76a367af57d38c0bc77086e784c2b1d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c092b3925ee7b5b7dbea29c528ad8db8.jpg\" _src=\"http://yanxuan.nosdn.127.net/c092b3925ee7b5b7dbea29c528ad8db8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aac2f3d5806016fb150d85bebc93b2e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/aac2f3d5806016fb150d85bebc93b2e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cfeb9a9bfcf4338db92e6d8709aef44.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cfeb9a9bfcf4338db92e6d8709aef44.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/453d3f8a6e61298886c3fa4361b59605.jpg\" _src=\"http://yanxuan.nosdn.127.net/453d3f8a6e61298886c3fa4361b59605.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d25fcc0a95baeba59f30b59afa3ff159.jpg\" _src=\"http://yanxuan.nosdn.127.net/d25fcc0a95baeba59f30b59afa3ff159.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ee00ea5c06c29973db9cf3c499ef0ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ee00ea5c06c29973db9cf3c499ef0ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23c51b8a7d25e88cc510609363f254a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/23c51b8a7d25e88cc510609363f254a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/07a632e4319a4cc45df6404975a4856a.jpg\" _src=\"http://yanxuan.nosdn.127.net/07a632e4319a4cc45df6404975a4856a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f20bda3dd2f724c3871226efc8ab3e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f20bda3dd2f724c3871226efc8ab3e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e237eaaad9484fa1ab1f4a8050df712.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e237eaaad9484fa1ab1f4a8050df712.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/68be7318cc3708254004b1f25abca889.jpg\" _src=\"http://yanxuan.nosdn.127.net/68be7318cc3708254004b1f25abca889.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c0aabf924bbb70486bb38bdf0fe0b9ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/c0aabf924bbb70486bb38bdf0fe0b9ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/938abacde4b46e5fce40c8cb6b5a31f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/938abacde4b46e5fce40c8cb6b5a31f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/560dc26811c85df2a81425ccc80f2daf.jpg\" _src=\"http://yanxuan.nosdn.127.net/560dc26811c85df2a81425ccc80f2daf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ea86c3ab570b110f24322dc88a2bf67c.jpg\" _src=\"http://yanxuan.nosdn.127.net/ea86c3ab570b110f24322dc88a2bf67c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20b35a848e5b3e68039d8825ebaf0a92.jpg\" _src=\"http://yanxuan.nosdn.127.net/20b35a848e5b3e68039d8825ebaf0a92.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/613568156bb735d4e826fadf9b14f30a.jpg\" _src=\"http://yanxuan.nosdn.127.net/613568156bb735d4e826fadf9b14f30a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c2626064e1a840a3fd0d8937092a2a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c2626064e1a840a3fd0d8937092a2a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4710cebed0fec2581f6c9d7a0ad35f4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/4710cebed0fec2581f6c9d7a0ad35f4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab23943bde5aee5a2f4db6305a638d06.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab23943bde5aee5a2f4db6305a638d06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f1722c1d44e6791a239d20ae2a84cb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f1722c1d44e6791a239d20ae2a84cb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec18f626b235961bba578d8726ab5d80.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec18f626b235961bba578d8726ab5d80.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f7c162a729f465edd62b2489af405820.jpg\" _src=\"http://yanxuan.nosdn.127.net/f7c162a729f465edd62b2489af405820.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de81035e3a2a44ad0420d25b374b248a.jpg\" _src=\"http://yanxuan.nosdn.127.net/de81035e3a2a44ad0420d25b374b248a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/92fcfcee4d8a828fcbda97ecd4ac7c61.jpg\" _src=\"http://yanxuan.nosdn.127.net/92fcfcee4d8a828fcbda97ecd4ac7c61.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c98e8d8abc2f97df7fa1ed3e8a19e793.jpg\" _src=\"http://yanxuan.nosdn.127.net/c98e8d8abc2f97df7fa1ed3e8a19e793.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/505355f028aafae9ac04ef604c46a89d.jpg\" _src=\"http://yanxuan.nosdn.127.net/505355f028aafae9ac04ef604c46a89d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3439e5f1fce7f602ae8fabce64e3bafa.jpg\" _src=\"http://yanxuan.nosdn.127.net/3439e5f1fce7f602ae8fabce64e3bafa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2ceea236ef9f0b2198dfce82e9265c06.jpg\" _src=\"http://yanxuan.nosdn.127.net/2ceea236ef9f0b2198dfce82e9265c06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/784fe3f5f7fdeebdb26b2dab8542d1f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/784fe3f5f7fdeebdb26b2dab8542d1f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15e4f99d5d272b0680868d2007d64382.jpg\" _src=\"http://yanxuan.nosdn.127.net/15e4f99d5d272b0680868d2007d64382.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99c09fe7b0d3ca49a81c7df0cc0a9dc1.jpg\" _src=\"http://yanxuan.nosdn.127.net/99c09fe7b0d3ca49a81c7df0cc0a9dc1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65c12643b55584e3e0474292c42088ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/65c12643b55584e3e0474292c42088ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d8d75b4b195d6086a44f2ee6d906d12.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d8d75b4b195d6086a44f2ee6d906d12.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c52456cd1b25174f0222273b7394a5b7.jpg\" _src=\"http://yanxuan.nosdn.127.net/c52456cd1b25174f0222273b7394a5b7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a089ad7a18777861c80d185b090dedc9.jpg\" _src=\"http://yanxuan.nosdn.127.net/a089ad7a18777861c80d185b090dedc9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/671ddba19da9b13492dbb5e3126fc018.jpg\" _src=\"http://yanxuan.nosdn.127.net/671ddba19da9b13492dbb5e3126fc018.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f60ed6e112c17e1ddbb301181477e8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f60ed6e112c17e1ddbb301181477e8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2a5a06bac71ceb645b47a322bef9588.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2a5a06bac71ceb645b47a322bef9588.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f612db88ffb6d1b7287039c8d3aee82d.jpg\" _src=\"http://yanxuan.nosdn.127.net/f612db88ffb6d1b7287039c8d3aee82d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27daed7f1faba0f42c1b0987eca43e1a.jpg\" _src=\"http://yanxuan.nosdn.127.net/27daed7f1faba0f42c1b0987eca43e1a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20a180e85c13f5ece01875ad91842193.jpg\" _src=\"http://yanxuan.nosdn.127.net/20a180e85c13f5ece01875ad91842193.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d42ca472ca07af1e8037673a2d1159e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d42ca472ca07af1e8037673a2d1159e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b161c4bf4b6937ed473449b21c61b8c.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b161c4bf4b6937ed473449b21c61b8c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76b268744bf751b5783ada179c343474.jpg\" _src=\"http://yanxuan.nosdn.127.net/76b268744bf751b5783ada179c343474.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18606e0a3c59f2a26585fbdd6a5dcedd.jpg\" _src=\"http://yanxuan.nosdn.127.net/18606e0a3c59f2a26585fbdd6a5dcedd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8636692d4819117b12b27f77506562d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/8636692d4819117b12b27f77506562d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b8d7e96b6cf7fc8dd7a4b9136c9c9c37.jpg\" _src=\"http://yanxuan.nosdn.127.net/b8d7e96b6cf7fc8dd7a4b9136c9c9c37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a69f5909a0ebf3450db5117530fbe339.jpg\" _src=\"http://yanxuan.nosdn.127.net/a69f5909a0ebf3450db5117530fbe339.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/00e9909b758d7585ac99423105b6d4a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/00e9909b758d7585ac99423105b6d4a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2ba5974ae02618ba26ff2bb17f3f13ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/2ba5974ae02618ba26ff2bb17f3f13ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9bea1ce19478453bbbe46607b7a7880c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9bea1ce19478453bbbe46607b7a7880c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ec70f25fdeab6b03b4b8f01dc070f5d4.jpg\" _src=\"http://yanxuan.nosdn.127.net/ec70f25fdeab6b03b4b8f01dc070f5d4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50bbfa868ba0fc8d424bf1ec82f78ac6.jpg\" _src=\"http://yanxuan.nosdn.127.net/50bbfa868ba0fc8d424bf1ec82f78ac6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b634157638fba9765dd10caf729e27e0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b634157638fba9765dd10caf729e27e0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79ccb6cc4a76e2b69976d3f279539b94.jpg\" _src=\"http://yanxuan.nosdn.127.net/79ccb6cc4a76e2b69976d3f279539b94.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 19,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a1f9e49a91ffda1505501d5015f30cda.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/442b9d99c0e7f39efd7967e0e5987374.png",
      "retail_price": 109,
      "sell_volume": 4383,
      "primary_product_id": 1130127,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1130042,
      "category_id": 1008002,
      "goods_sn": "1130042",
      "name": "皮毛一体多用单张长毛皮垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "盖毯、沙发垫、椅垫、地垫",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/d4ace79c311683de546aba0830b13cef.jpg\" _src=\"http://yanxuan.nosdn.127.net/d4ace79c311683de546aba0830b13cef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18f00b15f815b2d3b37f2348f51ce341.jpg\" _src=\"http://yanxuan.nosdn.127.net/18f00b15f815b2d3b37f2348f51ce341.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a17fcbf654cc3a60c107555af325f0fe.jpg\" _src=\"http://yanxuan.nosdn.127.net/a17fcbf654cc3a60c107555af325f0fe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6feee80476170267af6d71cdfc0b37dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6feee80476170267af6d71cdfc0b37dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/124b182a0a67835b4200cff8176c2b02.jpg\" _src=\"http://yanxuan.nosdn.127.net/124b182a0a67835b4200cff8176c2b02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd74be4a87738afaa04399b4d6d9a870.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd74be4a87738afaa04399b4d6d9a870.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e556cbed463186c4bd99726067b923af.jpg\" _src=\"http://yanxuan.nosdn.127.net/e556cbed463186c4bd99726067b923af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20688f897c671755758786d3040b5c07.jpg\" _src=\"http://yanxuan.nosdn.127.net/20688f897c671755758786d3040b5c07.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/260894bbf0796d65bebe0b8af28b6c95.jpg\" _src=\"http://yanxuan.nosdn.127.net/260894bbf0796d65bebe0b8af28b6c95.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/56c59db0a7a2edb57f79cd4ce4725ebd.jpg\" _src=\"http://yanxuan.nosdn.127.net/56c59db0a7a2edb57f79cd4ce4725ebd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f9abac8c992347562001de711510bb03.jpg\" _src=\"http://yanxuan.nosdn.127.net/f9abac8c992347562001de711510bb03.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1dfd5efde1a9607ad69344f3feb07cae.jpg\" _src=\"http://yanxuan.nosdn.127.net/1dfd5efde1a9607ad69344f3feb07cae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5563d9a3bcb3063e35ff0a04ea92e0f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/5563d9a3bcb3063e35ff0a04ea92e0f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7106f4f4495f0c3aea5174855ce2e54b.jpg\" _src=\"http://yanxuan.nosdn.127.net/7106f4f4495f0c3aea5174855ce2e54b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da4e5459ca9ce74f3ed0ff5c696d2893.jpg\" _src=\"http://yanxuan.nosdn.127.net/da4e5459ca9ce74f3ed0ff5c696d2893.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9b673bcc593d748b37a81edea189219.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9b673bcc593d748b37a81edea189219.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a72abb429df56c56bbe23b76f9b75204.jpg\" _src=\"http://yanxuan.nosdn.127.net/a72abb429df56c56bbe23b76f9b75204.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb1ba0a44c42710e55d6237a34d34ed6.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb1ba0a44c42710e55d6237a34d34ed6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/370e417d42332266cc31245eef4e2829.jpg\" _src=\"http://yanxuan.nosdn.127.net/370e417d42332266cc31245eef4e2829.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/604f40c00f0529e948a6f6823fe3f8e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/604f40c00f0529e948a6f6823fe3f8e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9ad179d3795a8ebd43f5c9572ba2164.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9ad179d3795a8ebd43f5c9572ba2164.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2cd302f653917f33d9a2d311599ed4f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/2cd302f653917f33d9a2d311599ed4f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da22ec1b12867fb95fd7614a7736f76c.jpg\" _src=\"http://yanxuan.nosdn.127.net/da22ec1b12867fb95fd7614a7736f76c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3671bc562ca4d94dc9b87ad90de08ef3.jpg\" _src=\"http://yanxuan.nosdn.127.net/3671bc562ca4d94dc9b87ad90de08ef3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/884bb79eb13e38ded605375476cc07e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/884bb79eb13e38ded605375476cc07e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f7fb86caeb445cf7eaf060f1df33383.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f7fb86caeb445cf7eaf060f1df33383.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/90680bb4193443696a79af88cc5786a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/90680bb4193443696a79af88cc5786a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ff03648c6839c642086a35143a0b5059.jpg\" _src=\"http://yanxuan.nosdn.127.net/ff03648c6839c642086a35143a0b5059.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f276b0dd0ca7fcdb576457a46eae4ff3.jpg\" _src=\"http://yanxuan.nosdn.127.net/f276b0dd0ca7fcdb576457a46eae4ff3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c7ec5147aee4c483754a957969029eb2.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7ec5147aee4c483754a957969029eb2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c26d9ad8701cc643cbfc6f69177791bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/c26d9ad8701cc643cbfc6f69177791bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55f4129b1fbcc20d6a0b9e2362043cb5.jpg\" _src=\"http://yanxuan.nosdn.127.net/55f4129b1fbcc20d6a0b9e2362043cb5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02770843341ed31eabb0ddadc5526c52.jpg\" _src=\"http://yanxuan.nosdn.127.net/02770843341ed31eabb0ddadc5526c52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd815b745f3c22fa4cff373d41943a86.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd815b745f3c22fa4cff373d41943a86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/480e0f3996285f44e368a73e6c5fe47d.jpg\" _src=\"http://yanxuan.nosdn.127.net/480e0f3996285f44e368a73e6c5fe47d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/264ee5efd645ca38168ad3bef5496cc5.jpg\" _src=\"http://yanxuan.nosdn.127.net/264ee5efd645ca38168ad3bef5496cc5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c46826b7d93342f359a818e80ec44765.jpg\" _src=\"http://yanxuan.nosdn.127.net/c46826b7d93342f359a818e80ec44765.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaade386233b7b54edadb80675494918.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaade386233b7b54edadb80675494918.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/848aac16cd9d30ce840deb70389c907b.jpg\" _src=\"http://yanxuan.nosdn.127.net/848aac16cd9d30ce840deb70389c907b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c50458c6772905734ff3e7ca1bce9978.jpg\" _src=\"http://yanxuan.nosdn.127.net/c50458c6772905734ff3e7ca1bce9978.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61834d14a5d1d2b77ac92e1baca558c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/61834d14a5d1d2b77ac92e1baca558c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/56ca8b2bc8f4b5ef00b2f87939a11602.jpg\" _src=\"http://yanxuan.nosdn.127.net/56ca8b2bc8f4b5ef00b2f87939a11602.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cb834323e30c14d86a4c1cc9b84d894.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cb834323e30c14d86a4c1cc9b84d894.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85e5f74e7205a9328209ca25be550598.jpg\" _src=\"http://yanxuan.nosdn.127.net/85e5f74e7205a9328209ca25be550598.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0ea202d5a703a4291495f5c0f83bed73.jpg\" _src=\"http://yanxuan.nosdn.127.net/0ea202d5a703a4291495f5c0f83bed73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf7433c7f8a437cf93ef90d1431adb57.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf7433c7f8a437cf93ef90d1431adb57.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbeddf135c0fe1f0ecfae5c6c057ea00.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbeddf135c0fe1f0ecfae5c6c057ea00.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/66b9e3c4986788281dece847560367d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/66b9e3c4986788281dece847560367d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e5d979ede709143d5f0f852855768c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e5d979ede709143d5f0f852855768c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce0a7f7bb447aa5148ecd03a7555c820.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce0a7f7bb447aa5148ecd03a7555c820.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e6b8abe385df7425ade75210724ffcc.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e6b8abe385df7425ade75210724ffcc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb3266c177f530869f44f1eaaf0b2bb7.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb3266c177f530869f44f1eaaf0b2bb7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ced47c9582a9353dc71d668467067b9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ced47c9582a9353dc71d668467067b9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae6270545f82ef2bee47fb0fa3d15e04.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae6270545f82ef2bee47fb0fa3d15e04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75d28b0323f8b9586d0339ab881c4e04.jpg\" _src=\"http://yanxuan.nosdn.127.net/75d28b0323f8b9586d0339ab881c4e04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d7750e85464204a7c57f50689eec1db4.jpg\" _src=\"http://yanxuan.nosdn.127.net/d7750e85464204a7c57f50689eec1db4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/373138262298b9c59e33a7cc3fe2f1e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/373138262298b9c59e33a7cc3fe2f1e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f39bae90e169f4e5417e0be5c66ad4df.jpg\" _src=\"http://yanxuan.nosdn.127.net/f39bae90e169f4e5417e0be5c66ad4df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f16ebd2501372da0d4b3e4e516df3fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f16ebd2501372da0d4b3e4e516df3fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f925d64a68d213867ceafc1211d59250.jpg\" _src=\"http://yanxuan.nosdn.127.net/f925d64a68d213867ceafc1211d59250.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eddd76fef80b87e1cf3a8d7bd6ceee3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/eddd76fef80b87e1cf3a8d7bd6ceee3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b74337d99199c178ff101a912cb37212.jpg\" _src=\"http://yanxuan.nosdn.127.net/b74337d99199c178ff101a912cb37212.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6fc6571f3526af0d9126071bd479e35.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6fc6571f3526af0d9126071bd479e35.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d26b83628f5e2b2830fd49b52ba67e70.jpg\" _src=\"http://yanxuan.nosdn.127.net/d26b83628f5e2b2830fd49b52ba67e70.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 20,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/e1d2090771d920c3feb477f07ac0ecb2.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/dc9d09334eb201fe9408ed604e549941.png",
      "retail_price": 239,
      "sell_volume": 4702,
      "primary_product_id": 1130130,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1134022,
      "category_id": 1008002,
      "goods_sn": "1134022",
      "name": "清新趣粉防滑浴垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "清新跃动，舒适脚感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/d68e182e560941e807d33431ad82452e.jpg\" _src=\"http://yanxuan.nosdn.127.net/d68e182e560941e807d33431ad82452e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/758e12cde995bc722cbab81644c29f60.jpg\" _src=\"http://yanxuan.nosdn.127.net/758e12cde995bc722cbab81644c29f60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b2cadfcad57975bc4b8ad4cb53ebbad.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b2cadfcad57975bc4b8ad4cb53ebbad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4600c0173de7dfa48d2c7d278667312f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4600c0173de7dfa48d2c7d278667312f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e766cfe5d9f6cf74390e37c271c5193.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e766cfe5d9f6cf74390e37c271c5193.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/97d7a034074e100db15b1c94f9f4308f.jpg\" _src=\"http://yanxuan.nosdn.127.net/97d7a034074e100db15b1c94f9f4308f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d78fd7ec09228ed93358f187b6c12398.jpg\" _src=\"http://yanxuan.nosdn.127.net/d78fd7ec09228ed93358f187b6c12398.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/00960ca0bd8f388fc52a493f39beac38.jpg\" _src=\"http://yanxuan.nosdn.127.net/00960ca0bd8f388fc52a493f39beac38.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb505efadcd8bb19d88b7ec1d86d5ade.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb505efadcd8bb19d88b7ec1d86d5ade.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/90ebd0a8cdd8a256b36fd26b2717a655.jpg\" _src=\"http://yanxuan.nosdn.127.net/90ebd0a8cdd8a256b36fd26b2717a655.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f391c39a3455577651ea1b2f7bb4832.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f391c39a3455577651ea1b2f7bb4832.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d153c03f2acc1e3062b507c135b309d6.jpg\" _src=\"http://yanxuan.nosdn.127.net/d153c03f2acc1e3062b507c135b309d6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9b6a5e8636dbfaa875b94c0221bf001.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9b6a5e8636dbfaa875b94c0221bf001.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dc971a8f5c766e3dd9f36fdfe6f9afd3.jpg\" _src=\"http://yanxuan.nosdn.127.net/dc971a8f5c766e3dd9f36fdfe6f9afd3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63dd064c791211bda9f0dfcf0bfe0db7.jpg\" _src=\"http://yanxuan.nosdn.127.net/63dd064c791211bda9f0dfcf0bfe0db7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15ecb7b4d9f3142a073eacd5506c0a2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/15ecb7b4d9f3142a073eacd5506c0a2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/278235956b0cd9a3aab8933c63c923c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/278235956b0cd9a3aab8933c63c923c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84bc90dec0c6f6049a79622f7b9ef83c.jpg\" _src=\"http://yanxuan.nosdn.127.net/84bc90dec0c6f6049a79622f7b9ef83c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9707c4a9a76f0432bb7c2d03b72f9582.jpg\" _src=\"http://yanxuan.nosdn.127.net/9707c4a9a76f0432bb7c2d03b72f9582.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3e75d69e0a16177a5b22a07ce0f39f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3e75d69e0a16177a5b22a07ce0f39f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ea585974061d0c9cc858bf5927f79cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ea585974061d0c9cc858bf5927f79cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aab2d28c54f55eddfeffb9fc7dc5e410.jpg\" _src=\"http://yanxuan.nosdn.127.net/aab2d28c54f55eddfeffb9fc7dc5e410.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9500f694389ca250f09b4f60d1be4f8.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9500f694389ca250f09b4f60d1be4f8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8f76b4a92255fdcccd1015476cf05b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8f76b4a92255fdcccd1015476cf05b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2247af207eb3872a7057f0d3dd0a9033.jpg\" _src=\"http://yanxuan.nosdn.127.net/2247af207eb3872a7057f0d3dd0a9033.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5b557985c26db27b73161505ee5d768.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5b557985c26db27b73161505ee5d768.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c16b77cdd7e12a597e2b8508cfc1e3e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/c16b77cdd7e12a597e2b8508cfc1e3e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1cf32a0024e223dd7e3953f642da5f4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/1cf32a0024e223dd7e3953f642da5f4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/594dca141f011e7cab4af1f7a19e19f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/594dca141f011e7cab4af1f7a19e19f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a52b1804711993bd96cdc9ca1ffcd10b.jpg\" _src=\"http://yanxuan.nosdn.127.net/a52b1804711993bd96cdc9ca1ffcd10b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/800bf6fc99f89ee6f0f8155fbd9accdb.jpg\" _src=\"http://yanxuan.nosdn.127.net/800bf6fc99f89ee6f0f8155fbd9accdb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55133777a4a7e79c0b13d31a81c077cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/55133777a4a7e79c0b13d31a81c077cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c5a4faf6e647754c6e364dfc4d5cbad.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c5a4faf6e647754c6e364dfc4d5cbad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18792955e7170d770c0f1cd559baee64.jpg\" _src=\"http://yanxuan.nosdn.127.net/18792955e7170d770c0f1cd559baee64.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2113fedc915eca6a7655f77d16f3a620.jpg\" _src=\"http://yanxuan.nosdn.127.net/2113fedc915eca6a7655f77d16f3a620.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4df06a31810e04bc083b71896ce9a326.jpg\" _src=\"http://yanxuan.nosdn.127.net/4df06a31810e04bc083b71896ce9a326.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29ce24ea1f9ba8c078b31aeaded6aa08.jpg\" _src=\"http://yanxuan.nosdn.127.net/29ce24ea1f9ba8c078b31aeaded6aa08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38e3bf328e84f4047a6d5fd4f66ac445.jpg\" _src=\"http://yanxuan.nosdn.127.net/38e3bf328e84f4047a6d5fd4f66ac445.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/956559986a2e62e87e6ba423964cd0f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/956559986a2e62e87e6ba423964cd0f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e79f219a7f9bbb98cbc7120a1699881e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e79f219a7f9bbb98cbc7120a1699881e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88ef1b4cc27eec82cbd38251be88f091.jpg\" _src=\"http://yanxuan.nosdn.127.net/88ef1b4cc27eec82cbd38251be88f091.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7261638f3f3a7287f150a20afdf4b66a.jpg\" _src=\"http://yanxuan.nosdn.127.net/7261638f3f3a7287f150a20afdf4b66a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebe2fcb1f43d47d335f139611bde77f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebe2fcb1f43d47d335f139611bde77f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7a153e2aaff1060fae1fd6ec41fdef9c.jpg\" _src=\"http://yanxuan.nosdn.127.net/7a153e2aaff1060fae1fd6ec41fdef9c.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 31,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/6e79581984d80627916b6e6035e5c6ae.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/a2b7489b4a2b1c09b66464cede4dabd7.png",
      "retail_price": 79,
      "sell_volume": 2166,
      "primary_product_id": 1135125,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1134030,
      "category_id": 1008002,
      "goods_sn": "1134030",
      "name": "简约知性记忆棉坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "慢回弹海绵，时尚设计。",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/3b31b3c57a7d7f42b13711bd1438d555.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b31b3c57a7d7f42b13711bd1438d555.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e92d9bad2a0339a81b47835f5530a358.jpg\" _src=\"http://yanxuan.nosdn.127.net/e92d9bad2a0339a81b47835f5530a358.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/edabc81fa6c7e66fe1698949f3b2b9f4.jpg\" _src=\"http://yanxuan.nosdn.127.net/edabc81fa6c7e66fe1698949f3b2b9f4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3444f640ec6ff6d6a8bcc3ce0f28848f.jpg\" _src=\"http://yanxuan.nosdn.127.net/3444f640ec6ff6d6a8bcc3ce0f28848f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/317ebb6f899631d1ed52759c14170a39.jpg\" _src=\"http://yanxuan.nosdn.127.net/317ebb6f899631d1ed52759c14170a39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f17af0ae3d56d482cec4105d390730a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f17af0ae3d56d482cec4105d390730a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/345a9aba507ca86b34c37c29956eeb83.jpg\" _src=\"http://yanxuan.nosdn.127.net/345a9aba507ca86b34c37c29956eeb83.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38b5c26064c4ea16ce3380bd69d2a671.jpg\" _src=\"http://yanxuan.nosdn.127.net/38b5c26064c4ea16ce3380bd69d2a671.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eabf8d6393d65cbd9e2e87c75dfcc066.jpg\" _src=\"http://yanxuan.nosdn.127.net/eabf8d6393d65cbd9e2e87c75dfcc066.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a703c316292e2c4c0b9d6551b25f1856.jpg\" _src=\"http://yanxuan.nosdn.127.net/a703c316292e2c4c0b9d6551b25f1856.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/734765425e21e073844c1c9e062dc35d.jpg\" _src=\"http://yanxuan.nosdn.127.net/734765425e21e073844c1c9e062dc35d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc24974d903f1d0e109482954f1da8e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc24974d903f1d0e109482954f1da8e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da57cdb5646fbff0cf8007f60304c30f.jpg\" _src=\"http://yanxuan.nosdn.127.net/da57cdb5646fbff0cf8007f60304c30f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddc76ceaeddfd7b527df40e01bf7877b.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddc76ceaeddfd7b527df40e01bf7877b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c158fdad4e3c80f90b02cf930b661bb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c158fdad4e3c80f90b02cf930b661bb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9682e656087dfa53c0f8365a0c300da.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9682e656087dfa53c0f8365a0c300da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/567cd1355b86120b192d36b4710552a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/567cd1355b86120b192d36b4710552a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/327629df66c47aeba0cb92072cf94471.jpg\" _src=\"http://yanxuan.nosdn.127.net/327629df66c47aeba0cb92072cf94471.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31199ec47d032c282762d8d49087c5af.jpg\" _src=\"http://yanxuan.nosdn.127.net/31199ec47d032c282762d8d49087c5af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/169746e1e8293452b58c184db111d98b.jpg\" _src=\"http://yanxuan.nosdn.127.net/169746e1e8293452b58c184db111d98b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a2a0cd32321cd198d67ea99fe5590120.jpg\" _src=\"http://yanxuan.nosdn.127.net/a2a0cd32321cd198d67ea99fe5590120.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4657e1914acce0c476d756f72e40ef97.jpg\" _src=\"http://yanxuan.nosdn.127.net/4657e1914acce0c476d756f72e40ef97.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9cb62e36a78ac61b587e6a9b5f9458a9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9cb62e36a78ac61b587e6a9b5f9458a9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b482df93b0a173be4a7bf6c2dabd543.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b482df93b0a173be4a7bf6c2dabd543.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/533e784b613baea6c7d18ea81ce3b535.jpg\" _src=\"http://yanxuan.nosdn.127.net/533e784b613baea6c7d18ea81ce3b535.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15772709fdda505c1a3a6b0e6453cce8.jpg\" _src=\"http://yanxuan.nosdn.127.net/15772709fdda505c1a3a6b0e6453cce8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b8ffb1a51ec50d46707513e6d6cb420.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b8ffb1a51ec50d46707513e6d6cb420.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cf3463a41c5fac921cdb11c3b0c8990.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cf3463a41c5fac921cdb11c3b0c8990.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2565c92fa398dd47a1458be3e9009c9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/2565c92fa398dd47a1458be3e9009c9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a4960bb2a74c1e22d82626ba7e33d33d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a4960bb2a74c1e22d82626ba7e33d33d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c13f2fb5d0daac9ef6fab890c866dc4.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c13f2fb5d0daac9ef6fab890c866dc4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/749704a3f974d419e8b59a32de540784.jpg\" _src=\"http://yanxuan.nosdn.127.net/749704a3f974d419e8b59a32de540784.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d1c4d8d91866700a5e8c1cd33ea75b15.jpg\" _src=\"http://yanxuan.nosdn.127.net/d1c4d8d91866700a5e8c1cd33ea75b15.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c55b8dc599470be31aa0218438a36528.jpg\" _src=\"http://yanxuan.nosdn.127.net/c55b8dc599470be31aa0218438a36528.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80c3a1e268905658a576eccd85a65f37.jpg\" _src=\"http://yanxuan.nosdn.127.net/80c3a1e268905658a576eccd85a65f37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c597a8dbecc1e3de31e9b8e5d420586.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c597a8dbecc1e3de31e9b8e5d420586.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/320ec6f1fcbb288e5676832dceff16aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/320ec6f1fcbb288e5676832dceff16aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8fc9119b2c7986bd575329d3a95abe9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8fc9119b2c7986bd575329d3a95abe9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/438a62f5bb789a6fa70b8ed5578cd7e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/438a62f5bb789a6fa70b8ed5578cd7e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1fe137a665f79a67359a9748de200ca6.jpg\" _src=\"http://yanxuan.nosdn.127.net/1fe137a665f79a67359a9748de200ca6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02ad092fac2cf5da935078f01afe3ff3.jpg\" _src=\"http://yanxuan.nosdn.127.net/02ad092fac2cf5da935078f01afe3ff3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d390285b49a6f4eb5ec9a460f77bce70.jpg\" _src=\"http://yanxuan.nosdn.127.net/d390285b49a6f4eb5ec9a460f77bce70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/469c7bc6e70c8d3db7639dc3d6949356.jpg\" _src=\"http://yanxuan.nosdn.127.net/469c7bc6e70c8d3db7639dc3d6949356.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/323b6604e88a5c748b4f7cd00ca84595.jpg\" _src=\"http://yanxuan.nosdn.127.net/323b6604e88a5c748b4f7cd00ca84595.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4151a8c4cae3b9998c95ae0bd9528e93.jpg\" _src=\"http://yanxuan.nosdn.127.net/4151a8c4cae3b9998c95ae0bd9528e93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c968e429b7a1f21ffa6281c76fd77c32.jpg\" _src=\"http://yanxuan.nosdn.127.net/c968e429b7a1f21ffa6281c76fd77c32.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 12,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 1,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/1f4758a9d68c5ebfafd3fc8b960707a6.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/aa49dfe878becf768eddc4c1636643a6.png",
      "retail_price": 46,
      "sell_volume": 7580,
      "primary_product_id": 1135146,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1134032,
      "category_id": 1008002,
      "goods_sn": "1134032",
      "name": "趣味粉彩系列记忆棉坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "慢回弹海绵的呵护，萌趣添彩。",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/ecbd6f05e8fc71571d889324e2f0dcad.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecbd6f05e8fc71571d889324e2f0dcad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bcdbec6d1b2ff457a0e7513df91563f0.jpg\" _src=\"http://yanxuan.nosdn.127.net/bcdbec6d1b2ff457a0e7513df91563f0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dcb21741c5c773e06cf4502925c81944.jpg\" _src=\"http://yanxuan.nosdn.127.net/dcb21741c5c773e06cf4502925c81944.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/86ffdbf55ae77e3c21a07a70445deda8.jpg\" _src=\"http://yanxuan.nosdn.127.net/86ffdbf55ae77e3c21a07a70445deda8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/598afa2e998b37d2c7513e7ab3a3ab73.jpg\" _src=\"http://yanxuan.nosdn.127.net/598afa2e998b37d2c7513e7ab3a3ab73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91dc47775ce962a1c2a7ac5e620f058c.jpg\" _src=\"http://yanxuan.nosdn.127.net/91dc47775ce962a1c2a7ac5e620f058c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/394b2bd47066e301a2144ab56b3b3350.jpg\" _src=\"http://yanxuan.nosdn.127.net/394b2bd47066e301a2144ab56b3b3350.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/80dd29542f2ecd571db647486cda4e9f.jpg\" _src=\"http://yanxuan.nosdn.127.net/80dd29542f2ecd571db647486cda4e9f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a5edf27fe34192ed741ee8b011e8bcc.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a5edf27fe34192ed741ee8b011e8bcc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d2ee6fd1f0893f6c033b27f7353d1622.jpg\" _src=\"http://yanxuan.nosdn.127.net/d2ee6fd1f0893f6c033b27f7353d1622.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e11dd4cdab417eba665e0ad4ebc9243e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e11dd4cdab417eba665e0ad4ebc9243e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/feb11e4b1fb22d07533f11b59d6e602f.jpg\" _src=\"http://yanxuan.nosdn.127.net/feb11e4b1fb22d07533f11b59d6e602f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5094e4cf95940490ffccfad5db698301.jpg\" _src=\"http://yanxuan.nosdn.127.net/5094e4cf95940490ffccfad5db698301.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b0f9af05048828816c9a774124509dd0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b0f9af05048828816c9a774124509dd0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82020ae739c4ba0957db83b22c102673.jpg\" _src=\"http://yanxuan.nosdn.127.net/82020ae739c4ba0957db83b22c102673.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09789518f58c163313d5d4b190888500.jpg\" _src=\"http://yanxuan.nosdn.127.net/09789518f58c163313d5d4b190888500.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d155f2f1d12b54e5dfc83e3d3496dc2.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d155f2f1d12b54e5dfc83e3d3496dc2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44d1b96c7810379c6b48d58e637cba55.jpg\" _src=\"http://yanxuan.nosdn.127.net/44d1b96c7810379c6b48d58e637cba55.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c2075c17cf5c447d27c89f23d2d63462.jpg\" _src=\"http://yanxuan.nosdn.127.net/c2075c17cf5c447d27c89f23d2d63462.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3985bdbdb5899bee08137ab2300f3810.jpg\" _src=\"http://yanxuan.nosdn.127.net/3985bdbdb5899bee08137ab2300f3810.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fe8a47c8056ed17d6e08ac715d3aee93.jpg\" _src=\"http://yanxuan.nosdn.127.net/fe8a47c8056ed17d6e08ac715d3aee93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31f98b129c846c333bb95db48c434271.jpg\" _src=\"http://yanxuan.nosdn.127.net/31f98b129c846c333bb95db48c434271.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/857e3041c75f5ffb2eeb394ca9e1211d.jpg\" _src=\"http://yanxuan.nosdn.127.net/857e3041c75f5ffb2eeb394ca9e1211d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b04c0a98d696e3ba0a37857bcca5ca4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b04c0a98d696e3ba0a37857bcca5ca4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33a9842b9e01b0629d56a4ae725611a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/33a9842b9e01b0629d56a4ae725611a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/296263f5dc5e365662203331a940d058.jpg\" _src=\"http://yanxuan.nosdn.127.net/296263f5dc5e365662203331a940d058.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25e32af7a35f9c3b1105d5e1dc163e8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/25e32af7a35f9c3b1105d5e1dc163e8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6efac795f3b6207cf090846887461d65.jpg\" _src=\"http://yanxuan.nosdn.127.net/6efac795f3b6207cf090846887461d65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9b1e2e1c90d1481c83460ff71eaa47e.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9b1e2e1c90d1481c83460ff71eaa47e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ab77215a79e8d9cc93304ec139af08e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ab77215a79e8d9cc93304ec139af08e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5eaab9336750bddb5a88fddfae7d2fbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/5eaab9336750bddb5a88fddfae7d2fbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e7046719cdf72538e69b0313587c8565.jpg\" _src=\"http://yanxuan.nosdn.127.net/e7046719cdf72538e69b0313587c8565.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/748836f2589106b87efec1c6be06f93d.jpg\" _src=\"http://yanxuan.nosdn.127.net/748836f2589106b87efec1c6be06f93d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40da8c4bed171c0fbfa9f2089a2309d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/40da8c4bed171c0fbfa9f2089a2309d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/468ed6ff0bbee10ba15467bb7b75c202.jpg\" _src=\"http://yanxuan.nosdn.127.net/468ed6ff0bbee10ba15467bb7b75c202.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2e1f9262f85b3301a6c9780acfcbb75.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2e1f9262f85b3301a6c9780acfcbb75.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ef0c70c73bff6274be4c562e88a7d6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ef0c70c73bff6274be4c562e88a7d6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/720c18b1bd787c125d59aa8f8f4c8e61.jpg\" _src=\"http://yanxuan.nosdn.127.net/720c18b1bd787c125d59aa8f8f4c8e61.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc80af1a2b58ac83a5d65cb3fa02f3db.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc80af1a2b58ac83a5d65cb3fa02f3db.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/98d647cacddc7bdd7eae86050eb9f3d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/98d647cacddc7bdd7eae86050eb9f3d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a091331dc2412de558446a42831b0358.jpg\" _src=\"http://yanxuan.nosdn.127.net/a091331dc2412de558446a42831b0358.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd6126e6eb2a4e493104f75ecbeb6e32.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd6126e6eb2a4e493104f75ecbeb6e32.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d15ad6abec2f8c499c0d9d036a8b524.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d15ad6abec2f8c499c0d9d036a8b524.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/69a56acc851dd042a52f18c78ac8ee33.jpg\" _src=\"http://yanxuan.nosdn.127.net/69a56acc851dd042a52f18c78ac8ee33.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8bde0e10b1e089088ca38fd77fbf994.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8bde0e10b1e089088ca38fd77fbf994.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd9ffb9b37957549689ece880fc78b2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd9ffb9b37957549689ece880fc78b2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09ad556caef32a5c951dc7fbad1f8de3.jpg\" _src=\"http://yanxuan.nosdn.127.net/09ad556caef32a5c951dc7fbad1f8de3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a919f989730d977f8b1745b5dc0e6a8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a919f989730d977f8b1745b5dc0e6a8d.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 13,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 1,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/5357e0476acbc71131df5a3fb3ea13d9.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/8b30eeb17c831eba08b97bdcb4c46a8e.png",
      "retail_price": 49,
      "sell_volume": 2869,
      "primary_product_id": 1135151,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135051,
      "category_id": 1008002,
      "goods_sn": "1135051",
      "name": "日式素雅纯色流星纹窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "日式素雅设计 流星纹简约肌理",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/70d4eceeb3f066bd4ea015fca75f424c.jpg\" _src=\"http://yanxuan.nosdn.127.net/70d4eceeb3f066bd4ea015fca75f424c.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebc7b596ef941847afe073a173bcfa59.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebc7b596ef941847afe073a173bcfa59.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c14d1ecbff1c587aefd16d65b47cae51.jpg\" _src=\"http://yanxuan.nosdn.127.net/c14d1ecbff1c587aefd16d65b47cae51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d269aeec1f4410c68b2f2c3f77f7985.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d269aeec1f4410c68b2f2c3f77f7985.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ae8263c89b5fbc0de5df0c21d67d3d2.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ae8263c89b5fbc0de5df0c21d67d3d2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/915f66ecc21197b4d99b5c3df5cbffab.jpg\" _src=\"http://yanxuan.nosdn.127.net/915f66ecc21197b4d99b5c3df5cbffab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4781c28a5295b239075883ccaa0a9c74.jpg\" _src=\"http://yanxuan.nosdn.127.net/4781c28a5295b239075883ccaa0a9c74.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91a4983796259d464e1f3795da189a17.jpg\" _src=\"http://yanxuan.nosdn.127.net/91a4983796259d464e1f3795da189a17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3950395fcc7e7fdc388a2ccf2b6ac0e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/3950395fcc7e7fdc388a2ccf2b6ac0e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9112abffdf6edd3b0ab8f9fb364d84f7.jpg\" _src=\"http://yanxuan.nosdn.127.net/9112abffdf6edd3b0ab8f9fb364d84f7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/96dcd6ccfec216bf2ce45393ca0aead1.jpg\" _src=\"http://yanxuan.nosdn.127.net/96dcd6ccfec216bf2ce45393ca0aead1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6dffe4e2cce9fb45abe1182bcb1939e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/6dffe4e2cce9fb45abe1182bcb1939e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d358645610f642ef7fd262c0101790e0.jpg\" _src=\"http://yanxuan.nosdn.127.net/d358645610f642ef7fd262c0101790e0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb51ccf74568565ba366f0eabf54ccbd.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb51ccf74568565ba366f0eabf54ccbd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7517d9dc2d70be25722a009083ed82df.jpg\" _src=\"http://yanxuan.nosdn.127.net/7517d9dc2d70be25722a009083ed82df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11deb1b2b5efa58291c8a62355df6017.jpg\" _src=\"http://yanxuan.nosdn.127.net/11deb1b2b5efa58291c8a62355df6017.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/172053c17a9a97a8108f8fd170a6b07f.jpg\" _src=\"http://yanxuan.nosdn.127.net/172053c17a9a97a8108f8fd170a6b07f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a1c0ac59021d408dcd9845c8702522a1.jpg\" _src=\"http://yanxuan.nosdn.127.net/a1c0ac59021d408dcd9845c8702522a1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/781d08f49d1870ac9cf8b93dacfbf711.jpg\" _src=\"http://yanxuan.nosdn.127.net/781d08f49d1870ac9cf8b93dacfbf711.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b764a61f92c6db3440f6b4aed6a7625.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b764a61f92c6db3440f6b4aed6a7625.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31ec911d03541ace9eddfbf3fcdf0414.jpg\" _src=\"http://yanxuan.nosdn.127.net/31ec911d03541ace9eddfbf3fcdf0414.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9d602c94b739bb01da939d75a9187a16.jpg\" _src=\"http://yanxuan.nosdn.127.net/9d602c94b739bb01da939d75a9187a16.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc557a3e4478f089973519699a01c01c.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc557a3e4478f089973519699a01c01c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1efdae30fe5189bb998509d446ff271.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1efdae30fe5189bb998509d446ff271.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/12116c10da83b5835a36315711640765.jpg\" _src=\"http://yanxuan.nosdn.127.net/12116c10da83b5835a36315711640765.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9491370cd9c5486fd9aa22ef9fdbd6fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/9491370cd9c5486fd9aa22ef9fdbd6fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37ca15cf48249bc390fcc05077741b98.jpg\" _src=\"http://yanxuan.nosdn.127.net/37ca15cf48249bc390fcc05077741b98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99fec7d83ae7e82a4426d3859875d8c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/99fec7d83ae7e82a4426d3859875d8c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9912fa7c176dc1b64c060992eb40b60.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9912fa7c176dc1b64c060992eb40b60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a04c0b364a1fa322ca6a71f35708e3ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/a04c0b364a1fa322ca6a71f35708e3ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8604f596b1d0703547d40608dfe16f2a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8604f596b1d0703547d40608dfe16f2a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b86422ab0ffe13da8f627245ec4dc98.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b86422ab0ffe13da8f627245ec4dc98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b2d3c68d23acb03a3c542cccb301bfb.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b2d3c68d23acb03a3c542cccb301bfb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d563205fb46fc71c3c37448673f5e714.jpg\" _src=\"http://yanxuan.nosdn.127.net/d563205fb46fc71c3c37448673f5e714.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18efa2d731c643a56a2976b4c793eec2.jpg\" _src=\"http://yanxuan.nosdn.127.net/18efa2d731c643a56a2976b4c793eec2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b644146188b5ceba4b86ec82352f660.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b644146188b5ceba4b86ec82352f660.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9c51c9c2c94f28102cb516656c7c761.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9c51c9c2c94f28102cb516656c7c761.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/769660ddc2ad27a1e62543460ff2bc41.jpg\" _src=\"http://yanxuan.nosdn.127.net/769660ddc2ad27a1e62543460ff2bc41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c95e64b4454063ba74c8cb17a95d60cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/c95e64b4454063ba74c8cb17a95d60cf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9a79d20d29a65bd010cf084c7b783d96.jpg\" _src=\"http://yanxuan.nosdn.127.net/9a79d20d29a65bd010cf084c7b783d96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18a89642689470308392fa485a633709.jpg\" _src=\"http://yanxuan.nosdn.127.net/18a89642689470308392fa485a633709.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/706c31eaec80f9417fbcdd40c16a7f63.jpg\" _src=\"http://yanxuan.nosdn.127.net/706c31eaec80f9417fbcdd40c16a7f63.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bec2e276673ab2787f03b8bd444044af.jpg\" _src=\"http://yanxuan.nosdn.127.net/bec2e276673ab2787f03b8bd444044af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3afb40257bc5fac38369dd465fe7732c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3afb40257bc5fac38369dd465fe7732c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5cfe30745d27efdc8080944bd8d8c927.jpg\" _src=\"http://yanxuan.nosdn.127.net/5cfe30745d27efdc8080944bd8d8c927.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e3aabaab6a42e859c2362998f235a564.jpg\" _src=\"http://yanxuan.nosdn.127.net/e3aabaab6a42e859c2362998f235a564.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6946e6dfe5a3026c67672c69061a06ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/6946e6dfe5a3026c67672c69061a06ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/778f89a8b141f03b6fcb206692b37d7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/778f89a8b141f03b6fcb206692b37d7f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b991c295b7bc2f6a6e04f7e79cede25.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b991c295b7bc2f6a6e04f7e79cede25.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e3f9724481dda6c024854750a3aeaa2.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e3f9724481dda6c024854750a3aeaa2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48bc347fe73c771d19787229da647421.jpg\" _src=\"http://yanxuan.nosdn.127.net/48bc347fe73c771d19787229da647421.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7a2a0bfe4036e4c3add5ba33313da069.jpg\" _src=\"http://yanxuan.nosdn.127.net/7a2a0bfe4036e4c3add5ba33313da069.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ec518bd9a7f9914841cc92e3e52fa45.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ec518bd9a7f9914841cc92e3e52fa45.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3054be42bc630607c3a46a9fe2ce6ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3054be42bc630607c3a46a9fe2ce6ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b368f5bd63b6b59b2064af102a1fa8e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b368f5bd63b6b59b2064af102a1fa8e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dda7a836f7a7c54256b35253bbfba90f.jpg\" _src=\"http://yanxuan.nosdn.127.net/dda7a836f7a7c54256b35253bbfba90f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91216189bef9aa48018bbf8e654443ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/91216189bef9aa48018bbf8e654443ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/10b8c1cace53090fe30a9834365ee37e.jpg\" _src=\"http://yanxuan.nosdn.127.net/10b8c1cace53090fe30a9834365ee37e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbf5782db6be5a01de6d0cf1c64eea30.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbf5782db6be5a01de6d0cf1c64eea30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c49df712817bfe30ec83a26af1b8b1de.jpg\" _src=\"http://yanxuan.nosdn.127.net/c49df712817bfe30ec83a26af1b8b1de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/510c05dc331823949d1567c552562a9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/510c05dc331823949d1567c552562a9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c673ce9d4d825503402f1c352b8e82ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/c673ce9d4d825503402f1c352b8e82ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/378135cf12f5c044871b59c060cacbb9.jpg\" _src=\"http://yanxuan.nosdn.127.net/378135cf12f5c044871b59c060cacbb9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd58aebd08f03474c7ed159c005a986c.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd58aebd08f03474c7ed159c005a986c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5a99049b512e9a388ffb1520827b2739.jpg\" _src=\"http://yanxuan.nosdn.127.net/5a99049b512e9a388ffb1520827b2739.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa65626e5df752d70ae4662d1b15dc8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa65626e5df752d70ae4662d1b15dc8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84d1dcf5083fd69abf4451a660f31d59.jpg\" _src=\"http://yanxuan.nosdn.127.net/84d1dcf5083fd69abf4451a660f31d59.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f781abaecbfb60889be6f46f83f4069.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f781abaecbfb60889be6f46f83f4069.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/26a745d26c76a4577feaf58b27ff557b.jpg\" _src=\"http://yanxuan.nosdn.127.net/26a745d26c76a4577feaf58b27ff557b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/887eb48649e1db53f3047340404209f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/887eb48649e1db53f3047340404209f6.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 35,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/95dbdb2e63eeed44c4a40ea586ad4196.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/9126151f028a8804026d530836b481cb.png",
      "retail_price": 299,
      "sell_volume": 1816,
      "primary_product_id": 1136377,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135052,
      "category_id": 1008002,
      "goods_sn": "1135052",
      "name": "日式简约素色窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "日式极简美学 舒适棉麻质感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/2edc19a016d64d3b29aa71b0bf6cc928.jpg\" _src=\"http://yanxuan.nosdn.127.net/2edc19a016d64d3b29aa71b0bf6cc928.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/6bdc1fc55629dbfccbdfaa6b17ebfacc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6bdc1fc55629dbfccbdfaa6b17ebfacc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4ef1e93a0d3f71d7862441ffd922e522.jpg\" _src=\"http://yanxuan.nosdn.127.net/4ef1e93a0d3f71d7862441ffd922e522.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85a1e175e39a6576dffb2f0ca28597f9.jpg\" _src=\"http://yanxuan.nosdn.127.net/85a1e175e39a6576dffb2f0ca28597f9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/486aedd7ce019d1c465bf8bbf77314bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/486aedd7ce019d1c465bf8bbf77314bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9f8f7045f07d1bb742f67120009afd0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9f8f7045f07d1bb742f67120009afd0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c813c0a23951007b020b9b03d0f31cb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c813c0a23951007b020b9b03d0f31cb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9a87cebbc5b127abf6a6e5129d4ed20c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9a87cebbc5b127abf6a6e5129d4ed20c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38e85411821a681c2dd5a5b9bd3cab92.jpg\" _src=\"http://yanxuan.nosdn.127.net/38e85411821a681c2dd5a5b9bd3cab92.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3907fa867c71f4090699898d53b937d.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3907fa867c71f4090699898d53b937d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c284309b66cc8d073f528c7ebf78c5fb.jpg\" _src=\"http://yanxuan.nosdn.127.net/c284309b66cc8d073f528c7ebf78c5fb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ecb27fc699a97883f7d14c7e606daa3.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ecb27fc699a97883f7d14c7e606daa3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eaf351d46c216f2f3a3588b3985d18c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/eaf351d46c216f2f3a3588b3985d18c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/785ab1ac578124415bbd718813413333.jpg\" _src=\"http://yanxuan.nosdn.127.net/785ab1ac578124415bbd718813413333.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8605647112b62e72f78ee27d29eede3d.jpg\" _src=\"http://yanxuan.nosdn.127.net/8605647112b62e72f78ee27d29eede3d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3952310896b95dcdc3adb986e5487a86.jpg\" _src=\"http://yanxuan.nosdn.127.net/3952310896b95dcdc3adb986e5487a86.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/030f115457262723b3d821987e38b111.jpg\" _src=\"http://yanxuan.nosdn.127.net/030f115457262723b3d821987e38b111.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf4254e1d4962d6e9f5e4734785f57ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf4254e1d4962d6e9f5e4734785f57ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce29d7cdc0e56477a623d03856646448.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce29d7cdc0e56477a623d03856646448.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/515086ca9168f8008291e98a01f4e4c9.jpg\" _src=\"http://yanxuan.nosdn.127.net/515086ca9168f8008291e98a01f4e4c9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9bb9d186d4a364ed0c91606d561a7f5.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9bb9d186d4a364ed0c91606d561a7f5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63204b444e0d06a7fafb6c5e35153eaa.jpg\" _src=\"http://yanxuan.nosdn.127.net/63204b444e0d06a7fafb6c5e35153eaa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d13212d5d43f766d3f5c37ccb4e5714.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d13212d5d43f766d3f5c37ccb4e5714.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19d5b4dbb590d90c3e40525a3ef35019.jpg\" _src=\"http://yanxuan.nosdn.127.net/19d5b4dbb590d90c3e40525a3ef35019.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0a1fcdbac2d1bf232e95389e20ed07c4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0a1fcdbac2d1bf232e95389e20ed07c4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d230fbda487cf445cd57f4296b7a487.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d230fbda487cf445cd57f4296b7a487.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5819e9bbdeda97281990f61c531fdbbb.jpg\" _src=\"http://yanxuan.nosdn.127.net/5819e9bbdeda97281990f61c531fdbbb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/802799f78d7069fc4dc44ff339729dc9.jpg\" _src=\"http://yanxuan.nosdn.127.net/802799f78d7069fc4dc44ff339729dc9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de5108481df4cbc2e064a1fcc477475f.jpg\" _src=\"http://yanxuan.nosdn.127.net/de5108481df4cbc2e064a1fcc477475f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a94262fecc2427d613ad7cbdd0a59f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a94262fecc2427d613ad7cbdd0a59f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b18c9c41d0520d1e0f1b58a7ae13e5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b18c9c41d0520d1e0f1b58a7ae13e5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/564d7115798352b765da2633949a1818.jpg\" _src=\"http://yanxuan.nosdn.127.net/564d7115798352b765da2633949a1818.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9f84553b8cfa29fb222b17bc89140fa9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9f84553b8cfa29fb222b17bc89140fa9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b01288738e632c5afda98184bb62095.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b01288738e632c5afda98184bb62095.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23088788bbfd7bf4b60ee06e9722ed74.jpg\" _src=\"http://yanxuan.nosdn.127.net/23088788bbfd7bf4b60ee06e9722ed74.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b2a400e968802cd64d31bdc038b3e2a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b2a400e968802cd64d31bdc038b3e2a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b0e31fe278c7704fed496ea82c679044.jpg\" _src=\"http://yanxuan.nosdn.127.net/b0e31fe278c7704fed496ea82c679044.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2054d55fc3bdaa380ce28c1fa9b4b00d.jpg\" _src=\"http://yanxuan.nosdn.127.net/2054d55fc3bdaa380ce28c1fa9b4b00d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4d03bae43ba821cd933d0e652e9d3bb7.jpg\" _src=\"http://yanxuan.nosdn.127.net/4d03bae43ba821cd933d0e652e9d3bb7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc1c458d99de149af69d8ac7582b72dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc1c458d99de149af69d8ac7582b72dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b92c88836f39dfc194d7e56cfdfcaf5c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b92c88836f39dfc194d7e56cfdfcaf5c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1446a01f9725a03ca79ab3e57fdc181a.jpg\" _src=\"http://yanxuan.nosdn.127.net/1446a01f9725a03ca79ab3e57fdc181a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/63fb7826d9f2d34f22317110d60a5b9d.jpg\" _src=\"http://yanxuan.nosdn.127.net/63fb7826d9f2d34f22317110d60a5b9d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/91b1dced907315eb0e771a504d29e6d7.jpg\" _src=\"http://yanxuan.nosdn.127.net/91b1dced907315eb0e771a504d29e6d7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/985d212a97d26d4ff1029ee4efdbc4f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/985d212a97d26d4ff1029ee4efdbc4f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8978ab0059b90f8b018b1de05fa4e8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8978ab0059b90f8b018b1de05fa4e8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25f62074f6e7e3e2b95a71e32aa43311.jpg\" _src=\"http://yanxuan.nosdn.127.net/25f62074f6e7e3e2b95a71e32aa43311.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9e8fa97196d22fb3bbc4cd871267cc79.jpg\" _src=\"http://yanxuan.nosdn.127.net/9e8fa97196d22fb3bbc4cd871267cc79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0c3478950cc4f473849ed3ab3de21bd4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0c3478950cc4f473849ed3ab3de21bd4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/838a150e46e5720a78f61ac48d380891.jpg\" _src=\"http://yanxuan.nosdn.127.net/838a150e46e5720a78f61ac48d380891.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2abd7db65b092e91ce87c09bf4c4c17f.jpg\" _src=\"http://yanxuan.nosdn.127.net/2abd7db65b092e91ce87c09bf4c4c17f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e603a799d802123ceaf5dbf3de02b051.jpg\" _src=\"http://yanxuan.nosdn.127.net/e603a799d802123ceaf5dbf3de02b051.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8460ba6d6347be878f035b7457ec9057.jpg\" _src=\"http://yanxuan.nosdn.127.net/8460ba6d6347be878f035b7457ec9057.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b02f932cfd15a19a2f1cebfab19b2cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b02f932cfd15a19a2f1cebfab19b2cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41fe9fb3c58a41023a74ef1740573fec.jpg\" _src=\"http://yanxuan.nosdn.127.net/41fe9fb3c58a41023a74ef1740573fec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19cc0338b0efefe7f0140efde638c705.jpg\" _src=\"http://yanxuan.nosdn.127.net/19cc0338b0efefe7f0140efde638c705.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e670a47f65733d99c4884f90b49d8e6.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e670a47f65733d99c4884f90b49d8e6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4859ec0aeecc39ed751f2a07daecad10.jpg\" _src=\"http://yanxuan.nosdn.127.net/4859ec0aeecc39ed751f2a07daecad10.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b7b2a56a1ea98119e89ae93b71e68c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b7b2a56a1ea98119e89ae93b71e68c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6e9767a0f40cbaf19307bd0c1ef97df9.jpg\" _src=\"http://yanxuan.nosdn.127.net/6e9767a0f40cbaf19307bd0c1ef97df9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ca04a1436a6598858fc74db1f571529.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ca04a1436a6598858fc74db1f571529.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/738fc25303e4bb32d1efe45641f1b120.jpg\" _src=\"http://yanxuan.nosdn.127.net/738fc25303e4bb32d1efe45641f1b120.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c5de7c6679cfe0361ac9d164276739ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/c5de7c6679cfe0361ac9d164276739ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e1edc1ea0bcc4cd92134ce8cc775577.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e1edc1ea0bcc4cd92134ce8cc775577.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e1eaacf6e5dc52fecb3e9c889db2ee32.jpg\" _src=\"http://yanxuan.nosdn.127.net/e1eaacf6e5dc52fecb3e9c889db2ee32.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/78cea538e5017c2782a96e215f42d6f3.jpg\" _src=\"http://yanxuan.nosdn.127.net/78cea538e5017c2782a96e215f42d6f3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f268a66c2e2476c075dd87416790b761.jpg\" _src=\"http://yanxuan.nosdn.127.net/f268a66c2e2476c075dd87416790b761.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9f6900f77c23e57a0a2633554ce0c8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9f6900f77c23e57a0a2633554ce0c8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9db7f3c92e24143e8ece310935785e41.jpg\" _src=\"http://yanxuan.nosdn.127.net/9db7f3c92e24143e8ece310935785e41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/923a8a571519b89b1a03e898871ef586.jpg\" _src=\"http://yanxuan.nosdn.127.net/923a8a571519b89b1a03e898871ef586.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 34,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/38129b4cdabcdf5610160d3a15ef259b.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/63f5da1f5363af43aa91864bf66af48e.png",
      "retail_price": 259,
      "sell_volume": 2776,
      "primary_product_id": 1136402,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135053,
      "category_id": 1008002,
      "goods_sn": "1135053",
      "name": "法式复古山形纹提花窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "轻奢复古，立体提花",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/e21a28b9c5e5203d217f54b0dec35735.jpg\" _src=\"http://yanxuan.nosdn.127.net/e21a28b9c5e5203d217f54b0dec35735.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/49e4de111eb6cf9ba70ee5ed8c85a416.jpg\" _src=\"http://yanxuan.nosdn.127.net/49e4de111eb6cf9ba70ee5ed8c85a416.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba9e72450a61c5259c0e025b155d58cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba9e72450a61c5259c0e025b155d58cf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41dc601d1494f0775e4763091a6671ca.jpg\" _src=\"http://yanxuan.nosdn.127.net/41dc601d1494f0775e4763091a6671ca.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d55bfd606020ef7de66bd70a1b93a12f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d55bfd606020ef7de66bd70a1b93a12f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bc7c6fa620e2635cced6ffbcfd4e6c49.jpg\" _src=\"http://yanxuan.nosdn.127.net/bc7c6fa620e2635cced6ffbcfd4e6c49.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a038525d854188e43cacd3ad2bf9a7a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/a038525d854188e43cacd3ad2bf9a7a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6224e8afea6653f1baaf9eceb70f4d1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/6224e8afea6653f1baaf9eceb70f4d1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/617f4b84e19adb6a5e81cf5c3a5574e1.jpg\" _src=\"http://yanxuan.nosdn.127.net/617f4b84e19adb6a5e81cf5c3a5574e1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5265f7746597699562be16e8cd367e78.jpg\" _src=\"http://yanxuan.nosdn.127.net/5265f7746597699562be16e8cd367e78.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7be914365886d471a418ca767e8b2432.jpg\" _src=\"http://yanxuan.nosdn.127.net/7be914365886d471a418ca767e8b2432.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2dce0091a62324d69685980ce463c8e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/2dce0091a62324d69685980ce463c8e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f190e680db954313c315ff788c2e677.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f190e680db954313c315ff788c2e677.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/349da9942e82dcc44629781ef2254c06.jpg\" _src=\"http://yanxuan.nosdn.127.net/349da9942e82dcc44629781ef2254c06.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9829be8b12dda40cec3c844df9e521b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/9829be8b12dda40cec3c844df9e521b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/082cb3197ad814c2df6f6089fa00fa46.jpg\" _src=\"http://yanxuan.nosdn.127.net/082cb3197ad814c2df6f6089fa00fa46.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca9038261114bdc03cb44ebabacaa67e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca9038261114bdc03cb44ebabacaa67e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5b4808db6982d4c6efb9967d3e0aad71.jpg\" _src=\"http://yanxuan.nosdn.127.net/5b4808db6982d4c6efb9967d3e0aad71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1b5f9b19c256980f8948b7eec4319f7e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1b5f9b19c256980f8948b7eec4319f7e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0fbe8e4222a5dbb5a34b774374377c60.jpg\" _src=\"http://yanxuan.nosdn.127.net/0fbe8e4222a5dbb5a34b774374377c60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3981672ef8bba7d656e1f6a439b2049.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3981672ef8bba7d656e1f6a439b2049.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/389a17a26b55ebd8090514087ed8b573.jpg\" _src=\"http://yanxuan.nosdn.127.net/389a17a26b55ebd8090514087ed8b573.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/577e2ba58b6c716b1f1e02d95992f8cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/577e2ba58b6c716b1f1e02d95992f8cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/deb4940d64591b194395c14f2d5407dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/deb4940d64591b194395c14f2d5407dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c0cce63ad9658252ddb9152a0801c69.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c0cce63ad9658252ddb9152a0801c69.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/51f7db1d8a7288aaf9712f978dd0e808.jpg\" _src=\"http://yanxuan.nosdn.127.net/51f7db1d8a7288aaf9712f978dd0e808.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09c3bdf807406fe5fe345e875ac4a69d.jpg\" _src=\"http://yanxuan.nosdn.127.net/09c3bdf807406fe5fe345e875ac4a69d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/818d25244f2dfdade6b23a4a92f55a51.jpg\" _src=\"http://yanxuan.nosdn.127.net/818d25244f2dfdade6b23a4a92f55a51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/310d4c4888d21f9100d36d7b19b7b841.jpg\" _src=\"http://yanxuan.nosdn.127.net/310d4c4888d21f9100d36d7b19b7b841.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb8e667ad88260e90211a4f9b246f8e4.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb8e667ad88260e90211a4f9b246f8e4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2b75ffc95e4a5c69944b99b7d3f04837.jpg\" _src=\"http://yanxuan.nosdn.127.net/2b75ffc95e4a5c69944b99b7d3f04837.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfef40e5a0861fb9e958b0a6a70c8cf8.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfef40e5a0861fb9e958b0a6a70c8cf8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a506fed177d609e43be43c4eb4ed0c6f.jpg\" _src=\"http://yanxuan.nosdn.127.net/a506fed177d609e43be43c4eb4ed0c6f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a6c905743a3c03c679c7017701399e1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/a6c905743a3c03c679c7017701399e1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2e44ac8c851c24ff28ef3d28fca1e363.jpg\" _src=\"http://yanxuan.nosdn.127.net/2e44ac8c851c24ff28ef3d28fca1e363.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d121846341c4eec125668560ea59606.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d121846341c4eec125668560ea59606.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbf82173395352acae173a6acac219c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbf82173395352acae173a6acac219c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8e6aff62f8304cf4c9847f1e6844407.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8e6aff62f8304cf4c9847f1e6844407.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a604d607f42ad8a1c343d604cc4c147.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a604d607f42ad8a1c343d604cc4c147.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/775d13d9704afa2a46ae2d6616ff78ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/775d13d9704afa2a46ae2d6616ff78ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65617bbfc95b22a4a6fb6060781afc70.jpg\" _src=\"http://yanxuan.nosdn.127.net/65617bbfc95b22a4a6fb6060781afc70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79613c75ad103b7b0cc1933a62afeff7.jpg\" _src=\"http://yanxuan.nosdn.127.net/79613c75ad103b7b0cc1933a62afeff7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9754dd885b4f1ff698b440d8582fda5b.jpg\" _src=\"http://yanxuan.nosdn.127.net/9754dd885b4f1ff698b440d8582fda5b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/372bbb746116a10e5c82d2c136883472.jpg\" _src=\"http://yanxuan.nosdn.127.net/372bbb746116a10e5c82d2c136883472.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79466f6b09420a3c8e8e39ab2091c32e.jpg\" _src=\"http://yanxuan.nosdn.127.net/79466f6b09420a3c8e8e39ab2091c32e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/852fce888e2e4abd8e9256207ce8857c.jpg\" _src=\"http://yanxuan.nosdn.127.net/852fce888e2e4abd8e9256207ce8857c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f51d785e3ecbe7da3abfb03527900ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f51d785e3ecbe7da3abfb03527900ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bdf18ac18c0bc4a9ca2834d14bc67e40.jpg\" _src=\"http://yanxuan.nosdn.127.net/bdf18ac18c0bc4a9ca2834d14bc67e40.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/64a9503d1375d2ce3cf2d3aaa8f49d0a.jpg\" _src=\"http://yanxuan.nosdn.127.net/64a9503d1375d2ce3cf2d3aaa8f49d0a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc7ea083ed7bee671c2b34fdf0a29837.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc7ea083ed7bee671c2b34fdf0a29837.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e58086a3385b0dcb915a35607e83a676.jpg\" _src=\"http://yanxuan.nosdn.127.net/e58086a3385b0dcb915a35607e83a676.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/239a602da7415684a44d5421ebb71e77.jpg\" _src=\"http://yanxuan.nosdn.127.net/239a602da7415684a44d5421ebb71e77.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c8ecca60b20a9f891c18adc051b7fbc.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c8ecca60b20a9f891c18adc051b7fbc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cf21f6ceb63279ceccbc35c882c9030c.jpg\" _src=\"http://yanxuan.nosdn.127.net/cf21f6ceb63279ceccbc35c882c9030c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7865fb8acee04157b94b85e62b6f2d14.jpg\" _src=\"http://yanxuan.nosdn.127.net/7865fb8acee04157b94b85e62b6f2d14.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3c1797e21327d8bff828ac761305867.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3c1797e21327d8bff828ac761305867.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d3263b186f04be03faa803dacf2bddcd.jpg\" _src=\"http://yanxuan.nosdn.127.net/d3263b186f04be03faa803dacf2bddcd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0a0bfa53b619a61d143314d60e13341.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0a0bfa53b619a61d143314d60e13341.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e3ddada3bf508947a5715df6792c980.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e3ddada3bf508947a5715df6792c980.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8ee6d2c940700caeec4997ff6deeca4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/8ee6d2c940700caeec4997ff6deeca4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3902aa67f3485894c892eef84be25952.jpg\" _src=\"http://yanxuan.nosdn.127.net/3902aa67f3485894c892eef84be25952.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9779fa93d513d2747aada4f83423df22.jpg\" _src=\"http://yanxuan.nosdn.127.net/9779fa93d513d2747aada4f83423df22.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4da023d34922ad0fc42ce5e4ac0e3431.jpg\" _src=\"http://yanxuan.nosdn.127.net/4da023d34922ad0fc42ce5e4ac0e3431.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5da0d3862a5e5f72b020a396fcc77423.jpg\" _src=\"http://yanxuan.nosdn.127.net/5da0d3862a5e5f72b020a396fcc77423.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f99a92c12c7057fd5dad948bb80cff98.jpg\" _src=\"http://yanxuan.nosdn.127.net/f99a92c12c7057fd5dad948bb80cff98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9453c191e802aeb86241cee2e2dd70a5.jpg\" _src=\"http://yanxuan.nosdn.127.net/9453c191e802aeb86241cee2e2dd70a5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/225ab93dd58a18f5878c57841c18b8ea.jpg\" _src=\"http://yanxuan.nosdn.127.net/225ab93dd58a18f5878c57841c18b8ea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/57994f32bd6423bed216a80c8456eafc.jpg\" _src=\"http://yanxuan.nosdn.127.net/57994f32bd6423bed216a80c8456eafc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9803612c814317b259e6c244fb3e191.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9803612c814317b259e6c244fb3e191.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 38,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/3235e120465f2755b6a412668d0be967.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/1f9e34b1aadd14ea0c9c299c530d86ba.png",
      "retail_price": 429,
      "sell_volume": 5280,
      "primary_product_id": 1136424,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135054,
      "category_id": 1008002,
      "goods_sn": "1135054",
      "name": "美式田园风蜻蜓提花窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "美式蜻蜓提花 甜美田园色彩",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/8b13ceefdeffbfd2b2326b9429ab7896.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b13ceefdeffbfd2b2326b9429ab7896.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8fa854947a7df61a4e063b8e2e14fd3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8fa854947a7df61a4e063b8e2e14fd3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d9681a7dd16355294e37057fa3b6c64.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d9681a7dd16355294e37057fa3b6c64.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/292b9704967295fcbf09ee7a98b40425.jpg\" _src=\"http://yanxuan.nosdn.127.net/292b9704967295fcbf09ee7a98b40425.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2ba9a3fb827a7c135670655ff4060553.jpg\" _src=\"http://yanxuan.nosdn.127.net/2ba9a3fb827a7c135670655ff4060553.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0b12070b3da9c44102a91b34d4a289d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0b12070b3da9c44102a91b34d4a289d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27a0e45f6cb8db4e541cc09dc3f56661.jpg\" _src=\"http://yanxuan.nosdn.127.net/27a0e45f6cb8db4e541cc09dc3f56661.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/78c39affb31ea084aec9092a528e1000.jpg\" _src=\"http://yanxuan.nosdn.127.net/78c39affb31ea084aec9092a528e1000.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1dbf236c3d1f41e23bb703be8e09d62.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1dbf236c3d1f41e23bb703be8e09d62.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8a10b18efc6670c4b5c6abfe25a5d791.jpg\" _src=\"http://yanxuan.nosdn.127.net/8a10b18efc6670c4b5c6abfe25a5d791.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31f310bfa2a088a865ba86d603c889e3.jpg\" _src=\"http://yanxuan.nosdn.127.net/31f310bfa2a088a865ba86d603c889e3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6e1112e5c699aadb80edf862b013241.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6e1112e5c699aadb80edf862b013241.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/70e35f2b7536dcf59061fb15e6fbd7f0.jpg\" _src=\"http://yanxuan.nosdn.127.net/70e35f2b7536dcf59061fb15e6fbd7f0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fab87a9493b50f6372eab5d02ab58ddc.jpg\" _src=\"http://yanxuan.nosdn.127.net/fab87a9493b50f6372eab5d02ab58ddc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6431ef7fa249e9e0412eceac99d77acb.jpg\" _src=\"http://yanxuan.nosdn.127.net/6431ef7fa249e9e0412eceac99d77acb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d6a3e40285e7e1ba47fff926acd7fb02.jpg\" _src=\"http://yanxuan.nosdn.127.net/d6a3e40285e7e1ba47fff926acd7fb02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d714470698ed5f14cf21ca34f3012bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d714470698ed5f14cf21ca34f3012bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9bc9c660db31968471b598a293b3c44b.jpg\" _src=\"http://yanxuan.nosdn.127.net/9bc9c660db31968471b598a293b3c44b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1bb7a825a3148cb187e8ec2d39b60f21.jpg\" _src=\"http://yanxuan.nosdn.127.net/1bb7a825a3148cb187e8ec2d39b60f21.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9097e4911884ae79e055d85ba0cc07b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/9097e4911884ae79e055d85ba0cc07b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/49195539f093b5974392cef9f3b2c5c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/49195539f093b5974392cef9f3b2c5c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71dc1d77d97e2495dea6edd66b62e906.jpg\" _src=\"http://yanxuan.nosdn.127.net/71dc1d77d97e2495dea6edd66b62e906.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbb3af413fa229c94682dea4e959edbe.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbb3af413fa229c94682dea4e959edbe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3a2b3bcda99806ff31844d44537f62e.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3a2b3bcda99806ff31844d44537f62e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e09dbf79c01d9ec02234be2063fade0.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e09dbf79c01d9ec02234be2063fade0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2838ac897fbc4339701789d3e05b176e.jpg\" _src=\"http://yanxuan.nosdn.127.net/2838ac897fbc4339701789d3e05b176e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/efe9c94a8e77081d69e8f30dfb501bc6.jpg\" _src=\"http://yanxuan.nosdn.127.net/efe9c94a8e77081d69e8f30dfb501bc6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2d8913b07b679efe4349802d9b0a6887.jpg\" _src=\"http://yanxuan.nosdn.127.net/2d8913b07b679efe4349802d9b0a6887.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aad09d61a369e2828a64996e6f594331.jpg\" _src=\"http://yanxuan.nosdn.127.net/aad09d61a369e2828a64996e6f594331.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09a0cc37d89dc0b604a69806ea1a1ec7.jpg\" _src=\"http://yanxuan.nosdn.127.net/09a0cc37d89dc0b604a69806ea1a1ec7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/680758fc7cf2315433ff5815b42a1620.jpg\" _src=\"http://yanxuan.nosdn.127.net/680758fc7cf2315433ff5815b42a1620.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6a83a5e81614a57ca3c55518130dc6e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/6a83a5e81614a57ca3c55518130dc6e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09474a7d70cb78b5baadd27906b09a48.jpg\" _src=\"http://yanxuan.nosdn.127.net/09474a7d70cb78b5baadd27906b09a48.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/85ffaf2d542e988adce23e576f539a11.jpg\" _src=\"http://yanxuan.nosdn.127.net/85ffaf2d542e988adce23e576f539a11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d56fded6471b21499e524b041fd7f409.jpg\" _src=\"http://yanxuan.nosdn.127.net/d56fded6471b21499e524b041fd7f409.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/01d319f088e87d2c3c223467de321352.jpg\" _src=\"http://yanxuan.nosdn.127.net/01d319f088e87d2c3c223467de321352.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2800c131d7320919b6b02adae7e5bd9.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2800c131d7320919b6b02adae7e5bd9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8172ab2121042e5703183b43fd195509.jpg\" _src=\"http://yanxuan.nosdn.127.net/8172ab2121042e5703183b43fd195509.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40dbb2286998622b9902fc704b583040.jpg\" _src=\"http://yanxuan.nosdn.127.net/40dbb2286998622b9902fc704b583040.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/68e4e99f2a0a400bfade8cd2befd0e69.jpg\" _src=\"http://yanxuan.nosdn.127.net/68e4e99f2a0a400bfade8cd2befd0e69.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba7ed53477cc0b34a0569704be78fb7a.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba7ed53477cc0b34a0569704be78fb7a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e1380ce14c595cc7c896ab6d80977c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e1380ce14c595cc7c896ab6d80977c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8625973becb30763b8185d5aed6ff2a.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8625973becb30763b8185d5aed6ff2a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/38d2ba1a53807474d5d1908c38e44941.jpg\" _src=\"http://yanxuan.nosdn.127.net/38d2ba1a53807474d5d1908c38e44941.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19c2742c33d946ea42525bb766b9aa50.jpg\" _src=\"http://yanxuan.nosdn.127.net/19c2742c33d946ea42525bb766b9aa50.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e38f6f972d9e0a5b1b929b00dac2ab7.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e38f6f972d9e0a5b1b929b00dac2ab7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2b39cc98245fb88155269d891af0165.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2b39cc98245fb88155269d891af0165.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf6dc932f82e427196f6202d1da99fc1.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf6dc932f82e427196f6202d1da99fc1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c90a23374fd5cf95dc05c0a687d52de7.jpg\" _src=\"http://yanxuan.nosdn.127.net/c90a23374fd5cf95dc05c0a687d52de7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c88e300269e108c04717dbd70539aa1e.jpg\" _src=\"http://yanxuan.nosdn.127.net/c88e300269e108c04717dbd70539aa1e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2c90271ed6fdd1b1cb114185962ac5b.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2c90271ed6fdd1b1cb114185962ac5b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/517fcab43dd3c867c9861835991185a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/517fcab43dd3c867c9861835991185a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/052b5796f383987f0982bfb21c62133d.jpg\" _src=\"http://yanxuan.nosdn.127.net/052b5796f383987f0982bfb21c62133d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/657fece964b17cdb783bce720165c81b.jpg\" _src=\"http://yanxuan.nosdn.127.net/657fece964b17cdb783bce720165c81b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3627ec2a160228289e561b4c4bad1c88.jpg\" _src=\"http://yanxuan.nosdn.127.net/3627ec2a160228289e561b4c4bad1c88.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c084cdba7d998c6026b77b2bedb16c8.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c084cdba7d998c6026b77b2bedb16c8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/609e6f0b7bcad8516f51c957c352e131.jpg\" _src=\"http://yanxuan.nosdn.127.net/609e6f0b7bcad8516f51c957c352e131.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b51e43dd314866fe7b8cf1def3896b5f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b51e43dd314866fe7b8cf1def3896b5f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f134c68159e3c4ae1b8cd31685c4a0da.jpg\" _src=\"http://yanxuan.nosdn.127.net/f134c68159e3c4ae1b8cd31685c4a0da.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d6c3dd50f40ce4d2f23e33a10af02f3.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d6c3dd50f40ce4d2f23e33a10af02f3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/93e670375dc312a0bce884d535b49543.jpg\" _src=\"http://yanxuan.nosdn.127.net/93e670375dc312a0bce884d535b49543.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e6ead1f50e3d5a5f7ece304975ebaf3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/e6ead1f50e3d5a5f7ece304975ebaf3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab5c9ba3fe26f2eac2908ff4ef0c3e38.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab5c9ba3fe26f2eac2908ff4ef0c3e38.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5955779f4196eacee871872e9c565237.jpg\" _src=\"http://yanxuan.nosdn.127.net/5955779f4196eacee871872e9c565237.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a54295c3a05ce118773f3b72a94ee198.jpg\" _src=\"http://yanxuan.nosdn.127.net/a54295c3a05ce118773f3b72a94ee198.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f0fb6a2b73c481dc8194efc9036daed.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f0fb6a2b73c481dc8194efc9036daed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bcffbd7e19cb83a129de0d1dcf70e3fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/bcffbd7e19cb83a129de0d1dcf70e3fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/533047cdb7474da59cb87adbe6c50e39.jpg\" _src=\"http://yanxuan.nosdn.127.net/533047cdb7474da59cb87adbe6c50e39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4aadd1564fd982d1f2267b49418441cf.jpg\" _src=\"http://yanxuan.nosdn.127.net/4aadd1564fd982d1f2267b49418441cf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71b5a16bc159955645369c89711374c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/71b5a16bc159955645369c89711374c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19a53b3e0bbbda6ee8dc2028930371a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/19a53b3e0bbbda6ee8dc2028930371a6.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 39,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/2f7641027f584b21e2f51d0a546291a0.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/30d7daa0824fbb61b6c36175c8203349.png",
      "retail_price": 559,
      "sell_volume": 22628,
      "primary_product_id": 1136431,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 1
    },
    {
      "id": 1135055,
      "category_id": 1008002,
      "goods_sn": "1135055",
      "name": "北欧印象几何条纹混色窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "山形纹提花 北欧简约混色",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/517a42ae18dfd98e7d3f311317ba3f54.jpg\" _src=\"http://yanxuan.nosdn.127.net/517a42ae18dfd98e7d3f311317ba3f54.jpg\"/><br/></p><p><img src=\"http://yanxuan.nosdn.127.net/68e9db2e8f912d4993a3c912e03f5f2c.jpg\" _src=\"http://yanxuan.nosdn.127.net/68e9db2e8f912d4993a3c912e03f5f2c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/41bc6c237355edd4d4e8dd89c504a4b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/41bc6c237355edd4d4e8dd89c504a4b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33f3534df43afd47eb9bb9e3cb85d0b0.jpg\" _src=\"http://yanxuan.nosdn.127.net/33f3534df43afd47eb9bb9e3cb85d0b0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/304afcf82a46055f14f62da9dbf079e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/304afcf82a46055f14f62da9dbf079e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b28ab088bc909f9964ce3dc6b911439.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b28ab088bc909f9964ce3dc6b911439.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31bb168618d29b6088bfe880a99934c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/31bb168618d29b6088bfe880a99934c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d965a3607b1a22f7f52e01261d7a507b.jpg\" _src=\"http://yanxuan.nosdn.127.net/d965a3607b1a22f7f52e01261d7a507b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f868badfd66ad1ed70fb7abc4a71f5b.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f868badfd66ad1ed70fb7abc4a71f5b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/662697d3bcdb8427452aec321d3e4c6a.jpg\" _src=\"http://yanxuan.nosdn.127.net/662697d3bcdb8427452aec321d3e4c6a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cdf2fd88a844f539f4c9873efb14a93d.jpg\" _src=\"http://yanxuan.nosdn.127.net/cdf2fd88a844f539f4c9873efb14a93d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1792cab519f6f0b489ddf95c30023f67.jpg\" _src=\"http://yanxuan.nosdn.127.net/1792cab519f6f0b489ddf95c30023f67.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/334801d2a30855b7bf207bf295b4ecfc.jpg\" _src=\"http://yanxuan.nosdn.127.net/334801d2a30855b7bf207bf295b4ecfc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2c18a7d948ec0ed09d777291a5f547ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/2c18a7d948ec0ed09d777291a5f547ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9bc0be56147bf743458d8df50fc5075f.jpg\" _src=\"http://yanxuan.nosdn.127.net/9bc0be56147bf743458d8df50fc5075f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f89950e36bc4c8ac8cb53e6b4377a9e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f89950e36bc4c8ac8cb53e6b4377a9e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3322ca38b778f0a9b3ac20a049cf520d.jpg\" _src=\"http://yanxuan.nosdn.127.net/3322ca38b778f0a9b3ac20a049cf520d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa487adfab5d685e9da06822a2ea5bb9.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa487adfab5d685e9da06822a2ea5bb9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23425bf14b340a87dcc22c9c4390e15e.jpg\" _src=\"http://yanxuan.nosdn.127.net/23425bf14b340a87dcc22c9c4390e15e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f1e82fc020816d3eb2ef17e24b9e5d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f1e82fc020816d3eb2ef17e24b9e5d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba7a8e956add1c16e9e49ca0d72bd30e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba7a8e956add1c16e9e49ca0d72bd30e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21635d8fed07731fe9d6e5a74bc69c41.jpg\" _src=\"http://yanxuan.nosdn.127.net/21635d8fed07731fe9d6e5a74bc69c41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ed0d59cbd62397d20b5fbf4626d41a93.jpg\" _src=\"http://yanxuan.nosdn.127.net/ed0d59cbd62397d20b5fbf4626d41a93.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/29d5b386af4b5f6a03996655d8295bae.jpg\" _src=\"http://yanxuan.nosdn.127.net/29d5b386af4b5f6a03996655d8295bae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0843c621c7f7d0d36cebcc5a1caf5d94.jpg\" _src=\"http://yanxuan.nosdn.127.net/0843c621c7f7d0d36cebcc5a1caf5d94.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bcb983612a08f762bd3bcc42dc98c709.jpg\" _src=\"http://yanxuan.nosdn.127.net/bcb983612a08f762bd3bcc42dc98c709.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7fe59f3d9cda66b0fd4a2c94e124d0ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/7fe59f3d9cda66b0fd4a2c94e124d0ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/31bd379ac7037b5e54ea93e4f8f833e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/31bd379ac7037b5e54ea93e4f8f833e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/331051a617e47532461c31e5ff7a16bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/331051a617e47532461c31e5ff7a16bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/443cd3bba1bc4e24a17801750b8ffd73.jpg\" _src=\"http://yanxuan.nosdn.127.net/443cd3bba1bc4e24a17801750b8ffd73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b408464b2167c203bd691c80badedeae.jpg\" _src=\"http://yanxuan.nosdn.127.net/b408464b2167c203bd691c80badedeae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79107afd183d1fe4429dd84e27b1869c.jpg\" _src=\"http://yanxuan.nosdn.127.net/79107afd183d1fe4429dd84e27b1869c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dcd5d9008ff6dbc93631ce29dab6b354.jpg\" _src=\"http://yanxuan.nosdn.127.net/dcd5d9008ff6dbc93631ce29dab6b354.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5f53f0045b4a770124615a12e724ced.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5f53f0045b4a770124615a12e724ced.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25ddf1a21d8d5a43ab3b1a5d505c65d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/25ddf1a21d8d5a43ab3b1a5d505c65d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbf4143559b00939a44fde123c8c2888.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbf4143559b00939a44fde123c8c2888.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2dac797df342a33a30e45e365ccbbfd9.jpg\" _src=\"http://yanxuan.nosdn.127.net/2dac797df342a33a30e45e365ccbbfd9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8c2564a0a643c338a3ba3ca6c7e7ff58.jpg\" _src=\"http://yanxuan.nosdn.127.net/8c2564a0a643c338a3ba3ca6c7e7ff58.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19cc6dc4032ac9ce30325fc92a5e345e.jpg\" _src=\"http://yanxuan.nosdn.127.net/19cc6dc4032ac9ce30325fc92a5e345e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb623f2b464c8cec997dc021a89571b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb623f2b464c8cec997dc021a89571b9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5bb40f61105e0380f7fec424ca29b1fa.jpg\" _src=\"http://yanxuan.nosdn.127.net/5bb40f61105e0380f7fec424ca29b1fa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/344edfec8435287400477554e2a4fcba.jpg\" _src=\"http://yanxuan.nosdn.127.net/344edfec8435287400477554e2a4fcba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9f33ab114476550b418a3f0fbaeea68.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9f33ab114476550b418a3f0fbaeea68.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b72c8e0a58bd04c363306fbd3bf429df.jpg\" _src=\"http://yanxuan.nosdn.127.net/b72c8e0a58bd04c363306fbd3bf429df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6a7308307c74336da7ff7330436a3dd6.jpg\" _src=\"http://yanxuan.nosdn.127.net/6a7308307c74336da7ff7330436a3dd6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b1086c39d44b373a2e8cdb3062d8c30.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b1086c39d44b373a2e8cdb3062d8c30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7c95781a9b95d7e01d384b410cb7a6a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c95781a9b95d7e01d384b410cb7a6a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd1f991f3beb2d9861df203c22a03b08.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd1f991f3beb2d9861df203c22a03b08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a55eccfd7e14fea5c551be5b94bf8851.jpg\" _src=\"http://yanxuan.nosdn.127.net/a55eccfd7e14fea5c551be5b94bf8851.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af209f2726ee582a11b0adf4473963bf.jpg\" _src=\"http://yanxuan.nosdn.127.net/af209f2726ee582a11b0adf4473963bf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb4b661f960dfab272a833732a338b84.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb4b661f960dfab272a833732a338b84.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0eac0f1694749e3f2ba7c3ce73234ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0eac0f1694749e3f2ba7c3ce73234ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9817135b6416cc72642ada8d285a22d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/9817135b6416cc72642ada8d285a22d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54443af2a33be3579ecfff18eeabb321.jpg\" _src=\"http://yanxuan.nosdn.127.net/54443af2a33be3579ecfff18eeabb321.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3f79c86438c27c8c0ad9511683fb900c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3f79c86438c27c8c0ad9511683fb900c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ebdc8e8f06f2fbe11bc2765038906df7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ebdc8e8f06f2fbe11bc2765038906df7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3e2cb3235a86089e75b3b848af26755e.jpg\" _src=\"http://yanxuan.nosdn.127.net/3e2cb3235a86089e75b3b848af26755e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2fef8703070e9b1be2e1367bb7c8ea00.jpg\" _src=\"http://yanxuan.nosdn.127.net/2fef8703070e9b1be2e1367bb7c8ea00.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c84eb4b1c7bb644faf451da2e2b0447.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c84eb4b1c7bb644faf451da2e2b0447.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7df41298392f5c0f38965e2b2097178a.jpg\" _src=\"http://yanxuan.nosdn.127.net/7df41298392f5c0f38965e2b2097178a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d458e8bf25e7c2877ed2b1ef5637aa9.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d458e8bf25e7c2877ed2b1ef5637aa9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/98cbb394e2b1cae7aaa848c85dd3af18.jpg\" _src=\"http://yanxuan.nosdn.127.net/98cbb394e2b1cae7aaa848c85dd3af18.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0e162e4742a0865e047b3e189591ae8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/0e162e4742a0865e047b3e189591ae8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4dfd24919e00f6c0715ce2323507c935.jpg\" _src=\"http://yanxuan.nosdn.127.net/4dfd24919e00f6c0715ce2323507c935.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/202ad04b025d49988cc0b4cabcca70f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/202ad04b025d49988cc0b4cabcca70f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b72277b67793dc6542783a2d0973869.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b72277b67793dc6542783a2d0973869.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75bceb04c01f9ebbe533a94b5eccb873.jpg\" _src=\"http://yanxuan.nosdn.127.net/75bceb04c01f9ebbe533a94b5eccb873.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/465b9fc2f115f3881e90120c738ece73.jpg\" _src=\"http://yanxuan.nosdn.127.net/465b9fc2f115f3881e90120c738ece73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/66dfd8708bd9d6ec229f56d22d1f1e82.jpg\" _src=\"http://yanxuan.nosdn.127.net/66dfd8708bd9d6ec229f56d22d1f1e82.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 37,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/0db87bc9137f5ca00f0d2de15a7cf607.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/87b6a608b99279ebf1764682e9e5fcec.png",
      "retail_price": 399,
      "sell_volume": 17157,
      "primary_product_id": 1136456,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135056,
      "category_id": 1008002,
      "goods_sn": "1135056",
      "name": "糖果色凹凸条纹儿童房窗帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "灵动色彩，童趣条纹",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/7c20355c62ad66dbba32b0e11f0f75d5.jpg\" _src=\"http://yanxuan.nosdn.127.net/7c20355c62ad66dbba32b0e11f0f75d5.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35552ca10129c4ec6530fbd5b3596f5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/35552ca10129c4ec6530fbd5b3596f5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba98905fc96c69c0a4bf4caec083be2f.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba98905fc96c69c0a4bf4caec083be2f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08f9e46394d65290533db13e32112890.jpg\" _src=\"http://yanxuan.nosdn.127.net/08f9e46394d65290533db13e32112890.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b16ba0cc72ef435e2999564ec20cf6c.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b16ba0cc72ef435e2999564ec20cf6c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/df3a97cb4c73bc9c1036bb0446368630.jpg\" _src=\"http://yanxuan.nosdn.127.net/df3a97cb4c73bc9c1036bb0446368630.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c6505b769f5c54f6e66231b03d9c9919.jpg\" _src=\"http://yanxuan.nosdn.127.net/c6505b769f5c54f6e66231b03d9c9919.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59a6179c8b6f523bc6c67646fcf0ca08.jpg\" _src=\"http://yanxuan.nosdn.127.net/59a6179c8b6f523bc6c67646fcf0ca08.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3b4ce480059631e26ffac109aa5d18c.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3b4ce480059631e26ffac109aa5d18c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/57dbe2baf75e5fa5529d1b3fd0ebdc97.jpg\" _src=\"http://yanxuan.nosdn.127.net/57dbe2baf75e5fa5529d1b3fd0ebdc97.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/72b5df8ead55acb75c626b7c4f22f76d.jpg\" _src=\"http://yanxuan.nosdn.127.net/72b5df8ead55acb75c626b7c4f22f76d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2a34c76a1a5bd369b0c7acf62813746a.jpg\" _src=\"http://yanxuan.nosdn.127.net/2a34c76a1a5bd369b0c7acf62813746a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c9fb571be38cc011c8edbaff7ab7c961.jpg\" _src=\"http://yanxuan.nosdn.127.net/c9fb571be38cc011c8edbaff7ab7c961.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae2f00a619449bbc968efbb99a0aacfd.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae2f00a619449bbc968efbb99a0aacfd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fe6dabb85692fd165279f626a27f9fb0.jpg\" _src=\"http://yanxuan.nosdn.127.net/fe6dabb85692fd165279f626a27f9fb0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f0e4d2016335e408106495abc2cf925.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f0e4d2016335e408106495abc2cf925.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfd6f2404e14e54f45f26baff796fca9.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfd6f2404e14e54f45f26baff796fca9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a034ad41437cb22dc27edeb8c7ced17c.jpg\" _src=\"http://yanxuan.nosdn.127.net/a034ad41437cb22dc27edeb8c7ced17c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d73f789cd190aaaf80d426939bfc4466.jpg\" _src=\"http://yanxuan.nosdn.127.net/d73f789cd190aaaf80d426939bfc4466.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a375c717468e02d130a3b335a469b4e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a375c717468e02d130a3b335a469b4e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3160e6ae5c4e0cf4809b0d7419c3bf5.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3160e6ae5c4e0cf4809b0d7419c3bf5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d0f8b77d9f28c35569d92d18f72c8c27.jpg\" _src=\"http://yanxuan.nosdn.127.net/d0f8b77d9f28c35569d92d18f72c8c27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b613b3604ded989f3aaeb1b3af5e7c60.jpg\" _src=\"http://yanxuan.nosdn.127.net/b613b3604ded989f3aaeb1b3af5e7c60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82d1d397861c98813e93876f878ed02a.jpg\" _src=\"http://yanxuan.nosdn.127.net/82d1d397861c98813e93876f878ed02a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/628c2aa615c30a97b2c43d829b75161f.jpg\" _src=\"http://yanxuan.nosdn.127.net/628c2aa615c30a97b2c43d829b75161f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/01899c4632878aa07b12e74b67259485.jpg\" _src=\"http://yanxuan.nosdn.127.net/01899c4632878aa07b12e74b67259485.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82554461e3615eea2564fbb9290e57ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/82554461e3615eea2564fbb9290e57ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/36b38aca196c62338811f878e18f52b4.jpg\" _src=\"http://yanxuan.nosdn.127.net/36b38aca196c62338811f878e18f52b4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a27d72b8fe9e3d533c8c448f7b4a0614.jpg\" _src=\"http://yanxuan.nosdn.127.net/a27d72b8fe9e3d533c8c448f7b4a0614.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e68d027072ddbb0420b21e3f0f44365.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e68d027072ddbb0420b21e3f0f44365.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c62bd7b6ce6ee1da5a27062df9363677.jpg\" _src=\"http://yanxuan.nosdn.127.net/c62bd7b6ce6ee1da5a27062df9363677.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76fde5b8b397c0efb12685fd8561123d.jpg\" _src=\"http://yanxuan.nosdn.127.net/76fde5b8b397c0efb12685fd8561123d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5816b3d9fae2b1d15fc462729fe977d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5816b3d9fae2b1d15fc462729fe977d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d57f643c8d33996708bab3052144aa99.jpg\" _src=\"http://yanxuan.nosdn.127.net/d57f643c8d33996708bab3052144aa99.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ecf67d3847b9050a377f751ce250ce34.jpg\" _src=\"http://yanxuan.nosdn.127.net/ecf67d3847b9050a377f751ce250ce34.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e01c7dc028bedd59001e7345a5a246d.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e01c7dc028bedd59001e7345a5a246d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4662d564c3b6df760dd19139a6af3060.jpg\" _src=\"http://yanxuan.nosdn.127.net/4662d564c3b6df760dd19139a6af3060.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2bab03382de1776e2cb9021947f44807.jpg\" _src=\"http://yanxuan.nosdn.127.net/2bab03382de1776e2cb9021947f44807.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/668e0c4505f9b86190207fe0d8be84ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/668e0c4505f9b86190207fe0d8be84ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19dbde9ef6edf5c1c8790049662287df.jpg\" _src=\"http://yanxuan.nosdn.127.net/19dbde9ef6edf5c1c8790049662287df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/53464274e000ef9c108a6875a4dc7a4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/53464274e000ef9c108a6875a4dc7a4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/138ff2f3f471cf84169a16730ac61c1a.jpg\" _src=\"http://yanxuan.nosdn.127.net/138ff2f3f471cf84169a16730ac61c1a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1397ec9bc1f099328c4991b1e1ba224d.jpg\" _src=\"http://yanxuan.nosdn.127.net/1397ec9bc1f099328c4991b1e1ba224d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/15ea2d7f9648e1e40915d3e300411994.jpg\" _src=\"http://yanxuan.nosdn.127.net/15ea2d7f9648e1e40915d3e300411994.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3011b59e959f2ef7f4ce50960b45af9c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3011b59e959f2ef7f4ce50960b45af9c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e74c96c5e3bb615176591afbb20d5b3.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e74c96c5e3bb615176591afbb20d5b3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fe8022ad7a0af1a1d3fd775789b43871.jpg\" _src=\"http://yanxuan.nosdn.127.net/fe8022ad7a0af1a1d3fd775789b43871.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb33363454d749da01e88d7f33d47637.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb33363454d749da01e88d7f33d47637.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b57a6785a7ca57472ead814b5e663ed9.jpg\" _src=\"http://yanxuan.nosdn.127.net/b57a6785a7ca57472ead814b5e663ed9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/58338bfd632396d37a32cc3a111e6d42.jpg\" _src=\"http://yanxuan.nosdn.127.net/58338bfd632396d37a32cc3a111e6d42.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f3d6d7f4d4e9fd6d4b7199ec3f993056.jpg\" _src=\"http://yanxuan.nosdn.127.net/f3d6d7f4d4e9fd6d4b7199ec3f993056.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e1bd19661b084036aef793cd04eb850.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e1bd19661b084036aef793cd04eb850.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a4a7ec58407e2c179a268c5f7d9f71b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a4a7ec58407e2c179a268c5f7d9f71b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b752ea0fa16847a196c7c72f9b3c790.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b752ea0fa16847a196c7c72f9b3c790.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b2b901ebaf68371b049d87036eb8f41f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b2b901ebaf68371b049d87036eb8f41f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f700d302dfb86c98afc8655526129c05.jpg\" _src=\"http://yanxuan.nosdn.127.net/f700d302dfb86c98afc8655526129c05.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb322b63a80aa3e44cca7d0c8fb06820.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb322b63a80aa3e44cca7d0c8fb06820.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d89b92178625b1c87406c1406c891aa7.jpg\" _src=\"http://yanxuan.nosdn.127.net/d89b92178625b1c87406c1406c891aa7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2e4a0c0718ab1f434af40220649c4776.jpg\" _src=\"http://yanxuan.nosdn.127.net/2e4a0c0718ab1f434af40220649c4776.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8cab72015ab23ae571eb8deb0f688870.jpg\" _src=\"http://yanxuan.nosdn.127.net/8cab72015ab23ae571eb8deb0f688870.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f9db276e7c5b8f81223da9bf2b81d146.jpg\" _src=\"http://yanxuan.nosdn.127.net/f9db276e7c5b8f81223da9bf2b81d146.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7e026d4db4dbdb745a970db7aab7a5ff.jpg\" _src=\"http://yanxuan.nosdn.127.net/7e026d4db4dbdb745a970db7aab7a5ff.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/abb53b015f71f95844b9b645f8d2a28e.jpg\" _src=\"http://yanxuan.nosdn.127.net/abb53b015f71f95844b9b645f8d2a28e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fae009fcecbb3b4d387519524f991457.jpg\" _src=\"http://yanxuan.nosdn.127.net/fae009fcecbb3b4d387519524f991457.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/05827553784f26cf0ccc6b02c3b1c7dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/05827553784f26cf0ccc6b02c3b1c7dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16d0bf68cd235dac5b72f47d4c7ace7f.jpg\" _src=\"http://yanxuan.nosdn.127.net/16d0bf68cd235dac5b72f47d4c7ace7f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/db55ff3fe3873426c8d047d3403387cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/db55ff3fe3873426c8d047d3403387cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/df067a032a8e3f85b7b1e9f3ae4a0ed6.jpg\" _src=\"http://yanxuan.nosdn.127.net/df067a032a8e3f85b7b1e9f3ae4a0ed6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a39eaca1d201e2f71f28c4ffa339e87a.jpg\" _src=\"http://yanxuan.nosdn.127.net/a39eaca1d201e2f71f28c4ffa339e87a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f9ff903bc8538e43ba0de5fcd57c3e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f9ff903bc8538e43ba0de5fcd57c3e2.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 36,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/5b9da3d72c73da202972f88ee1c7837b.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/536246ca4adb77274a94b18bb2f91f47.png",
      "retail_price": 259,
      "sell_volume": 10577,
      "primary_product_id": 1136472,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135057,
      "category_id": 1008002,
      "goods_sn": "1135057",
      "name": "梦幻系简约轻透莹白纱帘",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "轻透柔软纱 朦胧细纹肌理",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/088e63e0e298739ce0b7ad6aa4f3bc2d.jpg\" _src=\"http://yanxuan.nosdn.127.net/088e63e0e298739ce0b7ad6aa4f3bc2d.jpg\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44d08314b0c25796e5211b7f82d9c9cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/44d08314b0c25796e5211b7f82d9c9cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7a2aede16ff390bc980e8bd485e4e6a.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7a2aede16ff390bc980e8bd485e4e6a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb015656f9c0cf779739438143c7842d.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb015656f9c0cf779739438143c7842d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a76c38ce3e756deba85a09fe5551abcd.jpg\" _src=\"http://yanxuan.nosdn.127.net/a76c38ce3e756deba85a09fe5551abcd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f15917590cd0a049c095a2c95ccf832a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f15917590cd0a049c095a2c95ccf832a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1905c8981f963198da77643f3f774a54.jpg\" _src=\"http://yanxuan.nosdn.127.net/1905c8981f963198da77643f3f774a54.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2ccdfcf68dd4c0f908cfa5c48c76e3c.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2ccdfcf68dd4c0f908cfa5c48c76e3c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae6093e376c8ce4b008e5eef96cd2f6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae6093e376c8ce4b008e5eef96cd2f6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f5c6b8de674a14425396608d1788a6bc.jpg\" _src=\"http://yanxuan.nosdn.127.net/f5c6b8de674a14425396608d1788a6bc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aa9780ed9a8e1a744c589005428eccb3.jpg\" _src=\"http://yanxuan.nosdn.127.net/aa9780ed9a8e1a744c589005428eccb3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/814d1ee43b10292e38a838e32242ff95.jpg\" _src=\"http://yanxuan.nosdn.127.net/814d1ee43b10292e38a838e32242ff95.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbbe9bb7409bbc29285394c56fe6de65.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbbe9bb7409bbc29285394c56fe6de65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/001bc932cab905300c5c00a6da69db28.jpg\" _src=\"http://yanxuan.nosdn.127.net/001bc932cab905300c5c00a6da69db28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8bb1b60c6a52683d4d2689894ccbf20.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8bb1b60c6a52683d4d2689894ccbf20.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/817206ab2ffd7946e99f2c459bb725ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/817206ab2ffd7946e99f2c459bb725ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/557da67f50abfebb9f38c066ab7b202c.jpg\" _src=\"http://yanxuan.nosdn.127.net/557da67f50abfebb9f38c066ab7b202c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bf68d5bcaba0405d7a3043f7ea36663a.jpg\" _src=\"http://yanxuan.nosdn.127.net/bf68d5bcaba0405d7a3043f7ea36663a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/195cc13edfaaafa97d8f836e5d1c841a.jpg\" _src=\"http://yanxuan.nosdn.127.net/195cc13edfaaafa97d8f836e5d1c841a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27757a632a1b76e68b1ac520a2bfd5a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/27757a632a1b76e68b1ac520a2bfd5a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c24fe54ae36bd45b741a5ba8796113a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/c24fe54ae36bd45b741a5ba8796113a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/894a5ae76c69eb6759de91212a83fa04.jpg\" _src=\"http://yanxuan.nosdn.127.net/894a5ae76c69eb6759de91212a83fa04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b3aca05774b786d461645ec4faeefda.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b3aca05774b786d461645ec4faeefda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37293874fef9660e431fbe5d2f0a1fad.jpg\" _src=\"http://yanxuan.nosdn.127.net/37293874fef9660e431fbe5d2f0a1fad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3f6bb62defe913a888f049be018daa0.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3f6bb62defe913a888f049be018daa0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/35d2a4c32aa83b360cf60cb6a6c71d8f.jpg\" _src=\"http://yanxuan.nosdn.127.net/35d2a4c32aa83b360cf60cb6a6c71d8f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6758ccc43d3a31997bcdfedad718f6e3.jpg\" _src=\"http://yanxuan.nosdn.127.net/6758ccc43d3a31997bcdfedad718f6e3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d101a311f94525444c79075e6dc8a90f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d101a311f94525444c79075e6dc8a90f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1d336e42a2f94454ce0078be4389d4b2.jpg\" _src=\"http://yanxuan.nosdn.127.net/1d336e42a2f94454ce0078be4389d4b2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dae266d530a47edde62a0424b49cfe73.jpg\" _src=\"http://yanxuan.nosdn.127.net/dae266d530a47edde62a0424b49cfe73.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c2d1071f14177b19d292b6887544d6e.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c2d1071f14177b19d292b6887544d6e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e027ee3bc3fa0ced129d05dd85f629a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e027ee3bc3fa0ced129d05dd85f629a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5c56b8c566ae2dcc0697b4e7bb8b8630.jpg\" _src=\"http://yanxuan.nosdn.127.net/5c56b8c566ae2dcc0697b4e7bb8b8630.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be84eaf810654923eb06310883435942.jpg\" _src=\"http://yanxuan.nosdn.127.net/be84eaf810654923eb06310883435942.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b207cfccb4eda5a7278bd74c82adacda.jpg\" _src=\"http://yanxuan.nosdn.127.net/b207cfccb4eda5a7278bd74c82adacda.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54f86d151cf250d3a76a4cd725f9cdfe.jpg\" _src=\"http://yanxuan.nosdn.127.net/54f86d151cf250d3a76a4cd725f9cdfe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/44d3695e8dd5286b029aa7ce19a5b97a.jpg\" _src=\"http://yanxuan.nosdn.127.net/44d3695e8dd5286b029aa7ce19a5b97a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c80a2af6d1d1b40d382b1f495e83795.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c80a2af6d1d1b40d382b1f495e83795.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddd6008d180e884835cfd39094a81dd7.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddd6008d180e884835cfd39094a81dd7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b70b0bbb4933b57f7d28f517ef9c812.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b70b0bbb4933b57f7d28f517ef9c812.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/251f9ccb814f04ca5e6804b5ca60182f.jpg\" _src=\"http://yanxuan.nosdn.127.net/251f9ccb814f04ca5e6804b5ca60182f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad8ca0f8ffd3396ee1be6792b316d8fb.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad8ca0f8ffd3396ee1be6792b316d8fb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/96237772643462f0c923051df580ef8b.jpg\" _src=\"http://yanxuan.nosdn.127.net/96237772643462f0c923051df580ef8b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/054f71961df4fca4c0260d83a5d9bc98.jpg\" _src=\"http://yanxuan.nosdn.127.net/054f71961df4fca4c0260d83a5d9bc98.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d5cbcffbfcd3ac01e38eb3a01d0833a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/d5cbcffbfcd3ac01e38eb3a01d0833a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fb4bb9f35b500e7a0a7093ddbce407f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/fb4bb9f35b500e7a0a7093ddbce407f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/23a6091b704260334779826d2b858a9f.jpg\" _src=\"http://yanxuan.nosdn.127.net/23a6091b704260334779826d2b858a9f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aec34514179b3837429f6e4ab9f39759.jpg\" _src=\"http://yanxuan.nosdn.127.net/aec34514179b3837429f6e4ab9f39759.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/339a771531698027d36f917ccafadd02.jpg\" _src=\"http://yanxuan.nosdn.127.net/339a771531698027d36f917ccafadd02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/06def276699cc40e8f281c1f0b935c04.jpg\" _src=\"http://yanxuan.nosdn.127.net/06def276699cc40e8f281c1f0b935c04.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2648155e986745bf2269ef0857968bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2648155e986745bf2269ef0857968bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ef7a8e1db5aceba36645696895b04671.jpg\" _src=\"http://yanxuan.nosdn.127.net/ef7a8e1db5aceba36645696895b04671.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddb0d7fee5bde51071746aef961e28d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddb0d7fee5bde51071746aef961e28d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6752bad820840f5f0b684690d35f697d.jpg\" _src=\"http://yanxuan.nosdn.127.net/6752bad820840f5f0b684690d35f697d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aaec96a0239f848e38d79510191480a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/aaec96a0239f848e38d79510191480a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ad7d5c557d09e854388d33963566712e.jpg\" _src=\"http://yanxuan.nosdn.127.net/ad7d5c557d09e854388d33963566712e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d64a872b7b803ae2c6a3342edae85bb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/d64a872b7b803ae2c6a3342edae85bb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/859f290857188c448bdca0e20cf786ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/859f290857188c448bdca0e20cf786ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6cc76f812f3a2ebc107cc3d5e0c8da75.jpg\" _src=\"http://yanxuan.nosdn.127.net/6cc76f812f3a2ebc107cc3d5e0c8da75.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 33,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a007b270ec16a4d4c2c9e18d3b5cb06b.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/98c5e80b8e328687ce9c949314ebc41d.png",
      "retail_price": 199,
      "sell_volume": 4968,
      "primary_product_id": 1136484,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1135058,
      "category_id": 1008002,
      "goods_sn": "1135058",
      "name": "日式多功能手卷午睡枕坐垫",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "全棉针织条纹，透气按摩粒子",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/2286fb6b29d365466760ecbf2ebc8c82.jpg\" _src=\"http://yanxuan.nosdn.127.net/2286fb6b29d365466760ecbf2ebc8c82.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a9b2bd6e1049c5c4653a00b9802e6a11.jpg\" _src=\"http://yanxuan.nosdn.127.net/a9b2bd6e1049c5c4653a00b9802e6a11.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2639883802a55490ea81fe3dcd543df3.jpg\" _src=\"http://yanxuan.nosdn.127.net/2639883802a55490ea81fe3dcd543df3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/582b3658d2e405bd74dce301502d70f1.jpg\" _src=\"http://yanxuan.nosdn.127.net/582b3658d2e405bd74dce301502d70f1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ba9df33cbb0003bdab7d63dd0a70d599.jpg\" _src=\"http://yanxuan.nosdn.127.net/ba9df33cbb0003bdab7d63dd0a70d599.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/24c5d1905d9c31072445d87f7a37eebb.jpg\" _src=\"http://yanxuan.nosdn.127.net/24c5d1905d9c31072445d87f7a37eebb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e874eec46f85b846f696dd11fe61b858.jpg\" _src=\"http://yanxuan.nosdn.127.net/e874eec46f85b846f696dd11fe61b858.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d64ae710b7fc2c1cef03d7582515ede0.jpg\" _src=\"http://yanxuan.nosdn.127.net/d64ae710b7fc2c1cef03d7582515ede0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ab294e2889662c548e3e283e548d7ca2.jpg\" _src=\"http://yanxuan.nosdn.127.net/ab294e2889662c548e3e283e548d7ca2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2eb3eaef8f70960e95c67048faf1c68c.jpg\" _src=\"http://yanxuan.nosdn.127.net/2eb3eaef8f70960e95c67048faf1c68c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/11bf7eb8c196ecc361c963836b81d4ad.jpg\" _src=\"http://yanxuan.nosdn.127.net/11bf7eb8c196ecc361c963836b81d4ad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ef7b28262d2d7def40175ca98bde3222.jpg\" _src=\"http://yanxuan.nosdn.127.net/ef7b28262d2d7def40175ca98bde3222.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/678ae536ac582a2923cfa8240bf66aa8.jpg\" _src=\"http://yanxuan.nosdn.127.net/678ae536ac582a2923cfa8240bf66aa8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32d157099c01a5c6283513849f699d0f.jpg\" _src=\"http://yanxuan.nosdn.127.net/32d157099c01a5c6283513849f699d0f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e74c91fa555929d5493dcde5da877b02.jpg\" _src=\"http://yanxuan.nosdn.127.net/e74c91fa555929d5493dcde5da877b02.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e511841b236e95ab4ff0bf4562500ad0.jpg\" _src=\"http://yanxuan.nosdn.127.net/e511841b236e95ab4ff0bf4562500ad0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/deb067ad58dea4f11f53b191e3d1e77f.jpg\" _src=\"http://yanxuan.nosdn.127.net/deb067ad58dea4f11f53b191e3d1e77f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76a6d1fc324d373f70db08ce8750cb32.jpg\" _src=\"http://yanxuan.nosdn.127.net/76a6d1fc324d373f70db08ce8750cb32.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6305c83e95ddddd661cef3d5c9ac58cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/6305c83e95ddddd661cef3d5c9ac58cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c9dcf3269c87105f1841aed22d0f36fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/c9dcf3269c87105f1841aed22d0f36fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/54d7c9813569e17cef0f1027e5a52e6b.jpg\" _src=\"http://yanxuan.nosdn.127.net/54d7c9813569e17cef0f1027e5a52e6b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d39f00c7e20a5cd1a9ee8c9a65744cc0.jpg\" _src=\"http://yanxuan.nosdn.127.net/d39f00c7e20a5cd1a9ee8c9a65744cc0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b3bcd9d4b95c77f2a61dc5e29cd804cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3bcd9d4b95c77f2a61dc5e29cd804cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f52a276d2daf93cb61be8d6b6509106a.jpg\" _src=\"http://yanxuan.nosdn.127.net/f52a276d2daf93cb61be8d6b6509106a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d659bfb20371020a769309886aadd16f.jpg\" _src=\"http://yanxuan.nosdn.127.net/d659bfb20371020a769309886aadd16f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/43d05684abd3de808a8e35506a232c76.jpg\" _src=\"http://yanxuan.nosdn.127.net/43d05684abd3de808a8e35506a232c76.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48905901467d7f0950220b3eac766519.jpg\" _src=\"http://yanxuan.nosdn.127.net/48905901467d7f0950220b3eac766519.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ed5dcbd0e5d8b53cd6c4116780415af.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ed5dcbd0e5d8b53cd6c4116780415af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f0e8dbe1a4acb9985534c1a1017b91ce.jpg\" _src=\"http://yanxuan.nosdn.127.net/f0e8dbe1a4acb9985534c1a1017b91ce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5953f2c981375ea3945f368b9efcf2e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/5953f2c981375ea3945f368b9efcf2e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2afc692ecef8565da94ab96d605bd8d.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2afc692ecef8565da94ab96d605bd8d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b1c74ac52f6858cbaf6795bb98269a60.jpg\" _src=\"http://yanxuan.nosdn.127.net/b1c74ac52f6858cbaf6795bb98269a60.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c1090b13b82a36d182644a78c1ade112.jpg\" _src=\"http://yanxuan.nosdn.127.net/c1090b13b82a36d182644a78c1ade112.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8d28fba7b538217405ad66fb119e5fa0.jpg\" _src=\"http://yanxuan.nosdn.127.net/8d28fba7b538217405ad66fb119e5fa0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22588b3bc32226a798cb1ae6106525ae.jpg\" _src=\"http://yanxuan.nosdn.127.net/22588b3bc32226a798cb1ae6106525ae.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d9f07dcfdfa0e7a90df6e8c9ea397d17.jpg\" _src=\"http://yanxuan.nosdn.127.net/d9f07dcfdfa0e7a90df6e8c9ea397d17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/00df39022e7a1c29a9c0fbf4a0e3fb38.jpg\" _src=\"http://yanxuan.nosdn.127.net/00df39022e7a1c29a9c0fbf4a0e3fb38.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8588aabc1bbe4475026d74052b166a51.jpg\" _src=\"http://yanxuan.nosdn.127.net/8588aabc1bbe4475026d74052b166a51.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22071588ec58dfd880e913908acf2544.jpg\" _src=\"http://yanxuan.nosdn.127.net/22071588ec58dfd880e913908acf2544.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c8f02bcd66829318d9ca39618df2f42f.jpg\" _src=\"http://yanxuan.nosdn.127.net/c8f02bcd66829318d9ca39618df2f42f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0a72a74333e658a4da4bf886d74d739.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0a72a74333e658a4da4bf886d74d739.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e40a7ae5c9834f61408a1d31c839d79.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e40a7ae5c9834f61408a1d31c839d79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af4812a2debd12fb561816f2df84fddc.jpg\" _src=\"http://yanxuan.nosdn.127.net/af4812a2debd12fb561816f2df84fddc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e8182e35711a99d7e443bd69908948e2.jpg\" _src=\"http://yanxuan.nosdn.127.net/e8182e35711a99d7e443bd69908948e2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82ca0181ca502c76834e528135b272e8.jpg\" _src=\"http://yanxuan.nosdn.127.net/82ca0181ca502c76834e528135b272e8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f359915790a2bc8a399f243357da1cd4.jpg\" _src=\"http://yanxuan.nosdn.127.net/f359915790a2bc8a399f243357da1cd4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fa9246460b556890c5fdd5a8cc305743.jpg\" _src=\"http://yanxuan.nosdn.127.net/fa9246460b556890c5fdd5a8cc305743.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5381c329f434e08e18e087ebec952a28.jpg\" _src=\"http://yanxuan.nosdn.127.net/5381c329f434e08e18e087ebec952a28.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8f966701c7b93490c5cebf8e9cfdffa5.jpg\" _src=\"http://yanxuan.nosdn.127.net/8f966701c7b93490c5cebf8e9cfdffa5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/056d111c415c9db7282d8a27aeed9ae8.jpg\" _src=\"http://yanxuan.nosdn.127.net/056d111c415c9db7282d8a27aeed9ae8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/32dc1dbca7a4922e8da3aaf90ca5f1be.jpg\" _src=\"http://yanxuan.nosdn.127.net/32dc1dbca7a4922e8da3aaf90ca5f1be.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1ca114e5755a30f1557f8c75b89b1902.jpg\" _src=\"http://yanxuan.nosdn.127.net/1ca114e5755a30f1557f8c75b89b1902.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/959c4385428233e4ec256a6646ced133.jpg\" _src=\"http://yanxuan.nosdn.127.net/959c4385428233e4ec256a6646ced133.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 16,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/56fe8e4eda700613d852141b0fd22fa1.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/37bc0fa3524a904ac740340fa92bd515.png",
      "retail_price": 79,
      "sell_volume": 2023,
      "primary_product_id": 1136490,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1138000,
      "category_id": 1008002,
      "goods_sn": "1138000",
      "name": "日式蓬软太鼓抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "萌趣太鼓造型 软糯轻柔回弹",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/c0433bd3aafdc44b2b5fe10ced151823.jpg\" _src=\"http://yanxuan.nosdn.127.net/c0433bd3aafdc44b2b5fe10ced151823.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/241526b14e760f3b327d745127b7cadd.jpg\" _src=\"http://yanxuan.nosdn.127.net/241526b14e760f3b327d745127b7cadd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/924f6a3a78957b404ea2ad0ea24b4d58.jpg\" _src=\"http://yanxuan.nosdn.127.net/924f6a3a78957b404ea2ad0ea24b4d58.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/21b519690bf5574c6a4794fd0663fa37.jpg\" _src=\"http://yanxuan.nosdn.127.net/21b519690bf5574c6a4794fd0663fa37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/40ce0f2d0f0331024cb5eeffd48613f5.jpg\" _src=\"http://yanxuan.nosdn.127.net/40ce0f2d0f0331024cb5eeffd48613f5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/707d4c2e44903802f5181edc4d5e2aa4.jpg\" _src=\"http://yanxuan.nosdn.127.net/707d4c2e44903802f5181edc4d5e2aa4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0a26d87e0542007a59158a814b999f67.jpg\" _src=\"http://yanxuan.nosdn.127.net/0a26d87e0542007a59158a814b999f67.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5732b17001835e524acac7d3b75685e7.jpg\" _src=\"http://yanxuan.nosdn.127.net/5732b17001835e524acac7d3b75685e7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/19a4e7e34b7507e1ffb7ff3a3939a0fe.jpg\" _src=\"http://yanxuan.nosdn.127.net/19a4e7e34b7507e1ffb7ff3a3939a0fe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/699bf4c433ba2bb7736401e2272a2697.jpg\" _src=\"http://yanxuan.nosdn.127.net/699bf4c433ba2bb7736401e2272a2697.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb28a8cb46ffd42a39122d3f0724b3ee.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb28a8cb46ffd42a39122d3f0724b3ee.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/43f3eeb3661f54db929a9e3c8ee8be1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/43f3eeb3661f54db929a9e3c8ee8be1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37b4e61572b7c69462ae74b6a3cb4cb3.jpg\" _src=\"http://yanxuan.nosdn.127.net/37b4e61572b7c69462ae74b6a3cb4cb3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd17986d401a93b01526b7855e722efa.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd17986d401a93b01526b7855e722efa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e76a0c72a3e6cc2f15f61048ef1423c8.jpg\" _src=\"http://yanxuan.nosdn.127.net/e76a0c72a3e6cc2f15f61048ef1423c8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eabbdb77f25b449b1b3bcfd740a5c85c.jpg\" _src=\"http://yanxuan.nosdn.127.net/eabbdb77f25b449b1b3bcfd740a5c85c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c92f5747f156e0c3df3873456bfdc364.jpg\" _src=\"http://yanxuan.nosdn.127.net/c92f5747f156e0c3df3873456bfdc364.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fce1bbb0804c45fcedc0d407526197bd.jpg\" _src=\"http://yanxuan.nosdn.127.net/fce1bbb0804c45fcedc0d407526197bd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/de893522b3454e6769d46d5d16c35ec9.jpg\" _src=\"http://yanxuan.nosdn.127.net/de893522b3454e6769d46d5d16c35ec9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c7ca459ec92d9f32b25c4d1681a3efdf.jpg\" _src=\"http://yanxuan.nosdn.127.net/c7ca459ec92d9f32b25c4d1681a3efdf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd7974a599497d0830fe209f572f1d43.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd7974a599497d0830fe209f572f1d43.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a52672cac9385c1a6da086e46aead878.jpg\" _src=\"http://yanxuan.nosdn.127.net/a52672cac9385c1a6da086e46aead878.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/edc7589ef8d2d748b10d4fbe62d6cad9.jpg\" _src=\"http://yanxuan.nosdn.127.net/edc7589ef8d2d748b10d4fbe62d6cad9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/769529f68aad47685e9fd8ccc88a5065.jpg\" _src=\"http://yanxuan.nosdn.127.net/769529f68aad47685e9fd8ccc88a5065.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6151ae4dcae5a0ed3e9194c0d994e8d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/6151ae4dcae5a0ed3e9194c0d994e8d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddfb7e8eb34b476cb3a5cc6aeae1b414.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddfb7e8eb34b476cb3a5cc6aeae1b414.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/356742ded4619131733f009e7f44bdb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/356742ded4619131733f009e7f44bdb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d522efc0adefdf878a187d68287ccac7.jpg\" _src=\"http://yanxuan.nosdn.127.net/d522efc0adefdf878a187d68287ccac7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd385aa80f06967d8c120ee2a73ebdea.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd385aa80f06967d8c120ee2a73ebdea.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4a383ec27f0d0fecf6b218a6434a6537.jpg\" _src=\"http://yanxuan.nosdn.127.net/4a383ec27f0d0fecf6b218a6434a6537.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd76c5d83bdfac3eaef226032e9f2f1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd76c5d83bdfac3eaef226032e9f2f1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f37bf734bedcb5fc34f96a2d3ce21362.jpg\" _src=\"http://yanxuan.nosdn.127.net/f37bf734bedcb5fc34f96a2d3ce21362.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9426b170263b5f2e60b4e349002fb453.jpg\" _src=\"http://yanxuan.nosdn.127.net/9426b170263b5f2e60b4e349002fb453.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02c8fd2d4afb11e4ebfe7e675725f8b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/02c8fd2d4afb11e4ebfe7e675725f8b9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/55114d32fb55124afb57fa5f96c7aad6.jpg\" _src=\"http://yanxuan.nosdn.127.net/55114d32fb55124afb57fa5f96c7aad6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c812cb0cf47dfb2b0e0dbdd4e2ae2d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c812cb0cf47dfb2b0e0dbdd4e2ae2d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8491553451f68f13de7d88abd32e80bb.jpg\" _src=\"http://yanxuan.nosdn.127.net/8491553451f68f13de7d88abd32e80bb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2358865b0b2916d7b4c85105828e6f5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/2358865b0b2916d7b4c85105828e6f5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d4a761f631987bcb1542cee33c35661.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d4a761f631987bcb1542cee33c35661.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/af64442ed12ecc4ec0a8f1053f0e6c4f.jpg\" _src=\"http://yanxuan.nosdn.127.net/af64442ed12ecc4ec0a8f1053f0e6c4f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d00f1aa2e519c822a180024983611962.jpg\" _src=\"http://yanxuan.nosdn.127.net/d00f1aa2e519c822a180024983611962.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4dca882b9a0a583456f322030d96d99f.jpg\" _src=\"http://yanxuan.nosdn.127.net/4dca882b9a0a583456f322030d96d99f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a95ed3ffbb239954cc0f1089600847cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/a95ed3ffbb239954cc0f1089600847cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3783189e151670cae90114ac96208749.jpg\" _src=\"http://yanxuan.nosdn.127.net/3783189e151670cae90114ac96208749.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ea89e25888731072a7838f367efe40cc.jpg\" _src=\"http://yanxuan.nosdn.127.net/ea89e25888731072a7838f367efe40cc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1f3d87a044500179907d61e7984785b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/1f3d87a044500179907d61e7984785b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfc62369d2cebd727c24356199b3dfc6.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfc62369d2cebd727c24356199b3dfc6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/be23add374cfc9344889d449a537159c.jpg\" _src=\"http://yanxuan.nosdn.127.net/be23add374cfc9344889d449a537159c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/113f624f32c22d14b8fe49495d275bce.jpg\" _src=\"http://yanxuan.nosdn.127.net/113f624f32c22d14b8fe49495d275bce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ed060c62699d53a8d04451061aed0a95.jpg\" _src=\"http://yanxuan.nosdn.127.net/ed060c62699d53a8d04451061aed0a95.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a5cc33cd7c28a4c6dbb12e24c5b95e17.jpg\" _src=\"http://yanxuan.nosdn.127.net/a5cc33cd7c28a4c6dbb12e24c5b95e17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6ea47a643df6b81539cb50e83585febf.jpg\" _src=\"http://yanxuan.nosdn.127.net/6ea47a643df6b81539cb50e83585febf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37bd564f186c644e582eb5056597fe2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/37bd564f186c644e582eb5056597fe2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b47fe758560f31f84441a5420c2777e.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b47fe758560f31f84441a5420c2777e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/079946aa8f0edab416032a761e69c874.jpg\" _src=\"http://yanxuan.nosdn.127.net/079946aa8f0edab416032a761e69c874.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fab6ee083f738fe81e836f5b46345b8c.jpg\" _src=\"http://yanxuan.nosdn.127.net/fab6ee083f738fe81e836f5b46345b8c.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 2,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/afba3e98110e7a36dea74c5bdfe75e41.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ad953e16ad8c33b714e7af941ce8cd56.png",
      "retail_price": 29,
      "sell_volume": 49864,
      "primary_product_id": 1139013,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1138001,
      "category_id": 1008002,
      "goods_sn": "1138001",
      "name": "北欧简约山形纹绣花抱枕",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "精细刺绣，舒适立体",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/5737ca831d2cd44a2242eb0992583faf.jpg\" _src=\"http://yanxuan.nosdn.127.net/5737ca831d2cd44a2242eb0992583faf.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1160e68bcdeba98d2aada60af18c03c8.jpg\" _src=\"http://yanxuan.nosdn.127.net/1160e68bcdeba98d2aada60af18c03c8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c3772cb0d0f4767217726f9af7faa396.jpg\" _src=\"http://yanxuan.nosdn.127.net/c3772cb0d0f4767217726f9af7faa396.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/715a7f19500f5c28d9f73d37ebb1c557.jpg\" _src=\"http://yanxuan.nosdn.127.net/715a7f19500f5c28d9f73d37ebb1c557.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/84238cd8ab59b2fe193b825a3e89fd65.jpg\" _src=\"http://yanxuan.nosdn.127.net/84238cd8ab59b2fe193b825a3e89fd65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f4efe768f21095587d8bb4db202b2e23.jpg\" _src=\"http://yanxuan.nosdn.127.net/f4efe768f21095587d8bb4db202b2e23.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dbb5a935340a7ff61de6bec5fa3fd985.jpg\" _src=\"http://yanxuan.nosdn.127.net/dbb5a935340a7ff61de6bec5fa3fd985.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b0750c142e857a922d77999a48760cb9.jpg\" _src=\"http://yanxuan.nosdn.127.net/b0750c142e857a922d77999a48760cb9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d742c6ee8b65f2812784e13c2efd04fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/d742c6ee8b65f2812784e13c2efd04fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3aada66e84ec86907ca941fbc5235f12.jpg\" _src=\"http://yanxuan.nosdn.127.net/3aada66e84ec86907ca941fbc5235f12.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bb0fd8620c6d6208773667096709ba2b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bb0fd8620c6d6208773667096709ba2b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82b0a7a951c15b41eb5a4bb688dd74dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/82b0a7a951c15b41eb5a4bb688dd74dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/274fea6d222c1da9c687cb73f0f4f993.jpg\" _src=\"http://yanxuan.nosdn.127.net/274fea6d222c1da9c687cb73f0f4f993.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fc87ced2f7b274139bb079a75f7adf91.jpg\" _src=\"http://yanxuan.nosdn.127.net/fc87ced2f7b274139bb079a75f7adf91.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3a7f98096222daadf9820e1075670173.jpg\" _src=\"http://yanxuan.nosdn.127.net/3a7f98096222daadf9820e1075670173.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/26501a456d9e85980e12efe92120de56.jpg\" _src=\"http://yanxuan.nosdn.127.net/26501a456d9e85980e12efe92120de56.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7a9fbd6be2b2a3c2c83d4edaad2086a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/7a9fbd6be2b2a3c2c83d4edaad2086a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a3bf915e824b8b917c893167a99a3773.jpg\" _src=\"http://yanxuan.nosdn.127.net/a3bf915e824b8b917c893167a99a3773.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/211b5a457edcb05d3f3d21ff69c48398.jpg\" _src=\"http://yanxuan.nosdn.127.net/211b5a457edcb05d3f3d21ff69c48398.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cc0105d79ff4744f0680cbd2f87a8060.jpg\" _src=\"http://yanxuan.nosdn.127.net/cc0105d79ff4744f0680cbd2f87a8060.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f1da6da8c6b7b52f958fdec1dd7769c6.jpg\" _src=\"http://yanxuan.nosdn.127.net/f1da6da8c6b7b52f958fdec1dd7769c6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88ed21fc61da4f79545941fffce1f68c.jpg\" _src=\"http://yanxuan.nosdn.127.net/88ed21fc61da4f79545941fffce1f68c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6eb4abc57dbd46d6dcc38cac3bd32c68.jpg\" _src=\"http://yanxuan.nosdn.127.net/6eb4abc57dbd46d6dcc38cac3bd32c68.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c54b9b585c2e03559865e086f9b45bd.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c54b9b585c2e03559865e086f9b45bd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f88e9af10088b3a0b4669b27ef2fcadb.jpg\" _src=\"http://yanxuan.nosdn.127.net/f88e9af10088b3a0b4669b27ef2fcadb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6b249bac9bf3aa94bf4fffb5ac4d1e70.jpg\" _src=\"http://yanxuan.nosdn.127.net/6b249bac9bf3aa94bf4fffb5ac4d1e70.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b7ded1405eaa6f687eeb9e31b469d5de.jpg\" _src=\"http://yanxuan.nosdn.127.net/b7ded1405eaa6f687eeb9e31b469d5de.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3d072d1f04f7d94495227cf25b591744.jpg\" _src=\"http://yanxuan.nosdn.127.net/3d072d1f04f7d94495227cf25b591744.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/89f67b83d74f2a18b680bb5e6ef0d721.jpg\" _src=\"http://yanxuan.nosdn.127.net/89f67b83d74f2a18b680bb5e6ef0d721.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/236e948413b249b5ea4c1f6f8e835641.jpg\" _src=\"http://yanxuan.nosdn.127.net/236e948413b249b5ea4c1f6f8e835641.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b799d3613b5e3b87d89a608533473df8.jpg\" _src=\"http://yanxuan.nosdn.127.net/b799d3613b5e3b87d89a608533473df8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e6d4af8873253a0b5ae097c15c3628c0.jpg\" _src=\"http://yanxuan.nosdn.127.net/e6d4af8873253a0b5ae097c15c3628c0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fc017dc5a790385f6a96b43cf1a5b867.jpg\" _src=\"http://yanxuan.nosdn.127.net/fc017dc5a790385f6a96b43cf1a5b867.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0f10cc90e368fad0bd49fafc3b9047b5.jpg\" _src=\"http://yanxuan.nosdn.127.net/0f10cc90e368fad0bd49fafc3b9047b5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/864bf5646ba2ad778f507c224973bca7.jpg\" _src=\"http://yanxuan.nosdn.127.net/864bf5646ba2ad778f507c224973bca7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0443f772258e35af98be389a08fd85b8.jpg\" _src=\"http://yanxuan.nosdn.127.net/0443f772258e35af98be389a08fd85b8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/821926b210f311717fdaa0eccb142e37.jpg\" _src=\"http://yanxuan.nosdn.127.net/821926b210f311717fdaa0eccb142e37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/24d0ab5a259a662501e813cf21d752d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/24d0ab5a259a662501e813cf21d752d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b58c263c7e090c68d77e056c9d9afe27.jpg\" _src=\"http://yanxuan.nosdn.127.net/b58c263c7e090c68d77e056c9d9afe27.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d50d8b9f53f54ff0c066de7b39b2601c.jpg\" _src=\"http://yanxuan.nosdn.127.net/d50d8b9f53f54ff0c066de7b39b2601c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b382bfe1d8797e845bbcfd9dce361f76.jpg\" _src=\"http://yanxuan.nosdn.127.net/b382bfe1d8797e845bbcfd9dce361f76.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3aecb3e8d261312596727f56b54a0fa2.jpg\" _src=\"http://yanxuan.nosdn.127.net/3aecb3e8d261312596727f56b54a0fa2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c733463829f1fe8fa61998ae7c2ae37b.jpg\" _src=\"http://yanxuan.nosdn.127.net/c733463829f1fe8fa61998ae7c2ae37b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da2850f298b6cf4108e00a06bbc59821.jpg\" _src=\"http://yanxuan.nosdn.127.net/da2850f298b6cf4108e00a06bbc59821.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bd0924729a92af064c2108569e9d9463.jpg\" _src=\"http://yanxuan.nosdn.127.net/bd0924729a92af064c2108569e9d9463.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b819438a87396b0e3cc22202fc19caf0.jpg\" _src=\"http://yanxuan.nosdn.127.net/b819438a87396b0e3cc22202fc19caf0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3ea853201f8ad389ae3068f3d765aa44.jpg\" _src=\"http://yanxuan.nosdn.127.net/3ea853201f8ad389ae3068f3d765aa44.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5ef9093e1959a79178c32d5fc0fbe996.jpg\" _src=\"http://yanxuan.nosdn.127.net/5ef9093e1959a79178c32d5fc0fbe996.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da1d1a9a1e2afe85b640d573085a3d24.jpg\" _src=\"http://yanxuan.nosdn.127.net/da1d1a9a1e2afe85b640d573085a3d24.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ce702a9ac92d3666be5d4de2af5e03ab.jpg\" _src=\"http://yanxuan.nosdn.127.net/ce702a9ac92d3666be5d4de2af5e03ab.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b43f6da048bbc7206990d9ff972a23ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/b43f6da048bbc7206990d9ff972a23ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22eb869c0f07b55826e1e183dd498f3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/22eb869c0f07b55826e1e183dd498f3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d2c6bf7e29f0e8380ebef90b3bab2294.jpg\" _src=\"http://yanxuan.nosdn.127.net/d2c6bf7e29f0e8380ebef90b3bab2294.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 3,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/1d388fe2012c52f77732aef17b32a058.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/dbc5b25b824c3b3d7ff43b56ca35eee9.png",
      "retail_price": 79,
      "sell_volume": 5508,
      "primary_product_id": 1139049,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147045,
      "category_id": 1008002,
      "goods_sn": "1147045",
      "name": "清新趣粉系列居家地毯 灰黄条纹",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "条纹色块拼接 软糯温馨",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/baa3d2e8841117edfdf0b77ba4b923a3.jpg\" _src=\"http://yanxuan.nosdn.127.net/baa3d2e8841117edfdf0b77ba4b923a3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8c629e309184f5e1e51cdb10193bf993.jpg\" _src=\"http://yanxuan.nosdn.127.net/8c629e309184f5e1e51cdb10193bf993.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1e9f6e41af564fd0cc40a123dce69db4.jpg\" _src=\"http://yanxuan.nosdn.127.net/1e9f6e41af564fd0cc40a123dce69db4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/61df354d45227bd4d1870a792cc69b65.jpg\" _src=\"http://yanxuan.nosdn.127.net/61df354d45227bd4d1870a792cc69b65.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eb315d87c9b79db279e8fe1f0a4ff351.jpg\" _src=\"http://yanxuan.nosdn.127.net/eb315d87c9b79db279e8fe1f0a4ff351.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b43def579fe53f8b3d55f3838a5e98dc.jpg\" _src=\"http://yanxuan.nosdn.127.net/b43def579fe53f8b3d55f3838a5e98dc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4844c8fcd50ebca556d83c3b79563e30.jpg\" _src=\"http://yanxuan.nosdn.127.net/4844c8fcd50ebca556d83c3b79563e30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d8ec64be5f5e18d9c7c3f8031f843928.jpg\" _src=\"http://yanxuan.nosdn.127.net/d8ec64be5f5e18d9c7c3f8031f843928.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/76b3c0e01553f16457d2d86c7a4fcfd6.jpg\" _src=\"http://yanxuan.nosdn.127.net/76b3c0e01553f16457d2d86c7a4fcfd6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fef2ca1994a2fdb6a2ed15c6fcd55e71.jpg\" _src=\"http://yanxuan.nosdn.127.net/fef2ca1994a2fdb6a2ed15c6fcd55e71.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/02cc37f70c3eb52657303293f20d7273.jpg\" _src=\"http://yanxuan.nosdn.127.net/02cc37f70c3eb52657303293f20d7273.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e9970f5e3649225e7922cd16e2552f92.jpg\" _src=\"http://yanxuan.nosdn.127.net/e9970f5e3649225e7922cd16e2552f92.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/73be44d027e0869444fabcf8455f7c41.jpg\" _src=\"http://yanxuan.nosdn.127.net/73be44d027e0869444fabcf8455f7c41.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4b032b74be52d7f848073d847c4ad2e5.jpg\" _src=\"http://yanxuan.nosdn.127.net/4b032b74be52d7f848073d847c4ad2e5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39422d211ff45305b433f52be48ba594.jpg\" _src=\"http://yanxuan.nosdn.127.net/39422d211ff45305b433f52be48ba594.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/253b600c627a913f11621c4b0efabd9b.jpg\" _src=\"http://yanxuan.nosdn.127.net/253b600c627a913f11621c4b0efabd9b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e0615bcf15f2a5c242cf8ac8b25954e9.jpg\" _src=\"http://yanxuan.nosdn.127.net/e0615bcf15f2a5c242cf8ac8b25954e9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75c6bb3e19f57b854f3f1c81aebb12a5.jpg\" _src=\"http://yanxuan.nosdn.127.net/75c6bb3e19f57b854f3f1c81aebb12a5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0d8903b362c483a6a361e25db45efad4.jpg\" _src=\"http://yanxuan.nosdn.127.net/0d8903b362c483a6a361e25db45efad4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/861fb97fb4debc078419692924514e82.jpg\" _src=\"http://yanxuan.nosdn.127.net/861fb97fb4debc078419692924514e82.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/743398e0811fd6d35b89c8a381596b78.jpg\" _src=\"http://yanxuan.nosdn.127.net/743398e0811fd6d35b89c8a381596b78.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e9e0833fcc2817458548985fc82743a.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e9e0833fcc2817458548985fc82743a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6fc6a7297e038f54bdd793fa4d46b7f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/6fc6a7297e038f54bdd793fa4d46b7f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f9d1f2c5711307a84e2ef3a804eb124e.jpg\" _src=\"http://yanxuan.nosdn.127.net/f9d1f2c5711307a84e2ef3a804eb124e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d43ea14ec1e6a520d204fef585bc2ced.jpg\" _src=\"http://yanxuan.nosdn.127.net/d43ea14ec1e6a520d204fef585bc2ced.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca2cab985f7089ad1d6a94d6dd32ff79.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca2cab985f7089ad1d6a94d6dd32ff79.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/adaf13c5db73ab4617b6fa0523281cb8.jpg\" _src=\"http://yanxuan.nosdn.127.net/adaf13c5db73ab4617b6fa0523281cb8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7adf7694a6b17807ef8d209b762019ac.jpg\" _src=\"http://yanxuan.nosdn.127.net/7adf7694a6b17807ef8d209b762019ac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4e240ae9175c7038ba5aea852ba8d79b.jpg\" _src=\"http://yanxuan.nosdn.127.net/4e240ae9175c7038ba5aea852ba8d79b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f996a3aedda46c7035c7e62f15de1b12.jpg\" _src=\"http://yanxuan.nosdn.127.net/f996a3aedda46c7035c7e62f15de1b12.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b8d1f9feac00c6f0400cf1398075afe.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b8d1f9feac00c6f0400cf1398075afe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/da97979f5eb5ebc72258275a4dc4f811.jpg\" _src=\"http://yanxuan.nosdn.127.net/da97979f5eb5ebc72258275a4dc4f811.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/836c4651e2517b6fec9378f5b402ee52.jpg\" _src=\"http://yanxuan.nosdn.127.net/836c4651e2517b6fec9378f5b402ee52.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/aabd8aebb5ba1e110e83549fc4731695.jpg\" _src=\"http://yanxuan.nosdn.127.net/aabd8aebb5ba1e110e83549fc4731695.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9b9044c606ecc9f38abbf0221e3ebbd4.jpg\" _src=\"http://yanxuan.nosdn.127.net/9b9044c606ecc9f38abbf0221e3ebbd4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f16bc374ca38229922d2045a665e2748.jpg\" _src=\"http://yanxuan.nosdn.127.net/f16bc374ca38229922d2045a665e2748.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/71061c570c309fa87cc40be92015ddc2.jpg\" _src=\"http://yanxuan.nosdn.127.net/71061c570c309fa87cc40be92015ddc2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a96dbfd80979f937ea12a3af9320967f.jpg\" _src=\"http://yanxuan.nosdn.127.net/a96dbfd80979f937ea12a3af9320967f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/108f41fb93d0b1b4a126e5a9f1e4c36b.jpg\" _src=\"http://yanxuan.nosdn.127.net/108f41fb93d0b1b4a126e5a9f1e4c36b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/082055188b9b80a9280d87f0da63f071.jpg\" _src=\"http://yanxuan.nosdn.127.net/082055188b9b80a9280d87f0da63f071.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/16785ca3b958e7f7285e60d83cb642dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/16785ca3b958e7f7285e60d83cb642dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ddddc261de8e4000c8172e2541375167.jpg\" _src=\"http://yanxuan.nosdn.127.net/ddddc261de8e4000c8172e2541375167.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/59e2121b4fded2ec47e9b5465fd3e019.jpg\" _src=\"http://yanxuan.nosdn.127.net/59e2121b4fded2ec47e9b5465fd3e019.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/df574a0bb679353a6dc1fb0ddc5f3eb5.jpg\" _src=\"http://yanxuan.nosdn.127.net/df574a0bb679353a6dc1fb0ddc5f3eb5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/09ad34f2c245395cf95d6bfe90e178da.jpg\" _src=\"http://yanxuan.nosdn.127.net/09ad34f2c245395cf95d6bfe90e178da.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 28,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/4675b367076adc6817efd2b1f3746534.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/5cda4a0c4c4ff9728d03186bd053c9ca.png",
      "retail_price": 599,
      "sell_volume": 247,
      "primary_product_id": 1148174,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147046,
      "category_id": 1008002,
      "goods_sn": "1147046",
      "name": "清新趣粉系列居家地毯 条纹间粉",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "多色拼接 舒柔静音",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/b3e30fd4547bd74e73f6de777eb64bcd.jpg\" _src=\"http://yanxuan.nosdn.127.net/b3e30fd4547bd74e73f6de777eb64bcd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c224fa76981b3ee07645807d1ad0ab1c.jpg\" _src=\"http://yanxuan.nosdn.127.net/c224fa76981b3ee07645807d1ad0ab1c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77835aad8abf7f76f0c7d3a2733aae69.jpg\" _src=\"http://yanxuan.nosdn.127.net/77835aad8abf7f76f0c7d3a2733aae69.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2062742ccf38bdb099123db791cda7a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/2062742ccf38bdb099123db791cda7a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/952b3584258aae0d3e05ef6b62acdce5.jpg\" _src=\"http://yanxuan.nosdn.127.net/952b3584258aae0d3e05ef6b62acdce5.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d30e5094f3a9f6649d70680cbf0b3926.jpg\" _src=\"http://yanxuan.nosdn.127.net/d30e5094f3a9f6649d70680cbf0b3926.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b08dc18762700d9bf8cf76fbe25f2a5d.jpg\" _src=\"http://yanxuan.nosdn.127.net/b08dc18762700d9bf8cf76fbe25f2a5d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6c86c5e807cde9caeb442c7f38ec0150.jpg\" _src=\"http://yanxuan.nosdn.127.net/6c86c5e807cde9caeb442c7f38ec0150.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6d698add3680c26585135789f6017aac.jpg\" _src=\"http://yanxuan.nosdn.127.net/6d698add3680c26585135789f6017aac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/308bba84a93420ab84dcf137c1ed40cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/308bba84a93420ab84dcf137c1ed40cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d99cfdded9ca4eaf4b8893a02990a66e.jpg\" _src=\"http://yanxuan.nosdn.127.net/d99cfdded9ca4eaf4b8893a02990a66e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3fc5684fa24b379ab34a348305a771d8.jpg\" _src=\"http://yanxuan.nosdn.127.net/3fc5684fa24b379ab34a348305a771d8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/539f5536b64206e201ac52a9812685d9.jpg\" _src=\"http://yanxuan.nosdn.127.net/539f5536b64206e201ac52a9812685d9.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a9cb4fd76ff556c5d3dede50366c94e.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a9cb4fd76ff556c5d3dede50366c94e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4198d8a1ac1b9f8dec283041d4fd2995.jpg\" _src=\"http://yanxuan.nosdn.127.net/4198d8a1ac1b9f8dec283041d4fd2995.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/426ea47932152aea6bc507f3e7e45419.jpg\" _src=\"http://yanxuan.nosdn.127.net/426ea47932152aea6bc507f3e7e45419.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39a503db110fd6af417f2a4f8c69e0dd.jpg\" _src=\"http://yanxuan.nosdn.127.net/39a503db110fd6af417f2a4f8c69e0dd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/33c5cbd2a8b3f6e822411bd1c3ad7a8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/33c5cbd2a8b3f6e822411bd1c3ad7a8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08dc7ac6cf5bd20b14306161ad801f89.jpg\" _src=\"http://yanxuan.nosdn.127.net/08dc7ac6cf5bd20b14306161ad801f89.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dd0c4ae24186570c49ecb6ea6bc4d223.jpg\" _src=\"http://yanxuan.nosdn.127.net/dd0c4ae24186570c49ecb6ea6bc4d223.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/46eaed18b282b3177df608f9e410cfac.jpg\" _src=\"http://yanxuan.nosdn.127.net/46eaed18b282b3177df608f9e410cfac.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2e4a411c483653141471eec5c9c9f6fc.jpg\" _src=\"http://yanxuan.nosdn.127.net/2e4a411c483653141471eec5c9c9f6fc.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e013bfa3e6a997fcce4e526efa5d68fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/e013bfa3e6a997fcce4e526efa5d68fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50bc2637bd5ea29d1d787df548e494c3.jpg\" _src=\"http://yanxuan.nosdn.127.net/50bc2637bd5ea29d1d787df548e494c3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ef7aebd62895db555aec269d55cbe14a.jpg\" _src=\"http://yanxuan.nosdn.127.net/ef7aebd62895db555aec269d55cbe14a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cb53d78a085c29a0c12ec4c608db20a2.jpg\" _src=\"http://yanxuan.nosdn.127.net/cb53d78a085c29a0c12ec4c608db20a2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b887ad166e42363fe84e7a7a74971b88.jpg\" _src=\"http://yanxuan.nosdn.127.net/b887ad166e42363fe84e7a7a74971b88.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e57ab2325bfacc46a536d2e9f774814b.jpg\" _src=\"http://yanxuan.nosdn.127.net/e57ab2325bfacc46a536d2e9f774814b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2bf04434da86c3ef8f46e034164836a6.jpg\" _src=\"http://yanxuan.nosdn.127.net/2bf04434da86c3ef8f46e034164836a6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfa1f11efc7d868ae038fadc5f55096b.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfa1f11efc7d868ae038fadc5f55096b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0dd4b31cc78d7f9047948b224221b643.jpg\" _src=\"http://yanxuan.nosdn.127.net/0dd4b31cc78d7f9047948b224221b643.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39a3bc4e36427106682402c687addb1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/39a3bc4e36427106682402c687addb1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ae019d3a06a02983f26de10b3b415830.jpg\" _src=\"http://yanxuan.nosdn.127.net/ae019d3a06a02983f26de10b3b415830.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f8fef320814c866e80295655a8bcbd81.jpg\" _src=\"http://yanxuan.nosdn.127.net/f8fef320814c866e80295655a8bcbd81.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/980c7827076572b35c5c4c7bb2e65108.jpg\" _src=\"http://yanxuan.nosdn.127.net/980c7827076572b35c5c4c7bb2e65108.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/65f907cc355fe1701f3e2822bf631d55.jpg\" _src=\"http://yanxuan.nosdn.127.net/65f907cc355fe1701f3e2822bf631d55.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d27625f9111c8fd1bf19bc428b87a6d2.jpg\" _src=\"http://yanxuan.nosdn.127.net/d27625f9111c8fd1bf19bc428b87a6d2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/714ea85d22a65a2a7698a20ac9cb3320.jpg\" _src=\"http://yanxuan.nosdn.127.net/714ea85d22a65a2a7698a20ac9cb3320.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a8ee12c729cf07679d4135ac314c1b37.jpg\" _src=\"http://yanxuan.nosdn.127.net/a8ee12c729cf07679d4135ac314c1b37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0bcb12fdd8d835705ee9ac88b764b441.jpg\" _src=\"http://yanxuan.nosdn.127.net/0bcb12fdd8d835705ee9ac88b764b441.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79124540860c5a26842803b62b46fc8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/79124540860c5a26842803b62b46fc8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca54c7438b6cfe4c139f9a07e9c0b055.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca54c7438b6cfe4c139f9a07e9c0b055.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a4eede58b9d7b516b708bd1bfb18e9df.jpg\" _src=\"http://yanxuan.nosdn.127.net/a4eede58b9d7b516b708bd1bfb18e9df.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/25db36db73d7b38380b3c829a12770d3.jpg\" _src=\"http://yanxuan.nosdn.127.net/25db36db73d7b38380b3c829a12770d3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c86f1f43a2cc6f25c0d162601fa143b9.jpg\" _src=\"http://yanxuan.nosdn.127.net/c86f1f43a2cc6f25c0d162601fa143b9.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 26,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/a4ec154d8a8496dd4aa490c8ec6f8bfd.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/655d718df8107f8e7fd1dc6140e29039.png",
      "retail_price": 599,
      "sell_volume": 225,
      "primary_product_id": 1148175,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147047,
      "category_id": 1008002,
      "goods_sn": "1147047",
      "name": "简约知性系列居家地毯 蓝粉拼接",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "三角几何拼接 超细绒感",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/e56e30a2c6cbdeadb1a2b6d00f2e877f.jpg\" _src=\"http://yanxuan.nosdn.127.net/e56e30a2c6cbdeadb1a2b6d00f2e877f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/d14496c74886e92b3a3f30692756e77a.jpg\" _src=\"http://yanxuan.nosdn.127.net/d14496c74886e92b3a3f30692756e77a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0a371e340849de0ca0c628021cbc0014.jpg\" _src=\"http://yanxuan.nosdn.127.net/0a371e340849de0ca0c628021cbc0014.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a5a80c783e941991414cd8ede724312.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a5a80c783e941991414cd8ede724312.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/37a49c90311b2661a24887ff2de448c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/37a49c90311b2661a24887ff2de448c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e25787020a28bbb6e9f2a220aa2dd442.jpg\" _src=\"http://yanxuan.nosdn.127.net/e25787020a28bbb6e9f2a220aa2dd442.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/52b8beb545c2ae0115522908ac352a39.jpg\" _src=\"http://yanxuan.nosdn.127.net/52b8beb545c2ae0115522908ac352a39.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/afaa8978308f2531ada6aaaf63c56347.jpg\" _src=\"http://yanxuan.nosdn.127.net/afaa8978308f2531ada6aaaf63c56347.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/18789d3aacac9d2de6a6b21cfb7aec53.jpg\" _src=\"http://yanxuan.nosdn.127.net/18789d3aacac9d2de6a6b21cfb7aec53.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/154e9f3504ada7cdadcb906ee01450c7.jpg\" _src=\"http://yanxuan.nosdn.127.net/154e9f3504ada7cdadcb906ee01450c7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3326e16fbfee855392404e970bd5aa4c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3326e16fbfee855392404e970bd5aa4c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7b5b0d22fc526776cef8e756dff60dd1.jpg\" _src=\"http://yanxuan.nosdn.127.net/7b5b0d22fc526776cef8e756dff60dd1.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/48dd357aa1abc60c01b3fbf8dacb2694.jpg\" _src=\"http://yanxuan.nosdn.127.net/48dd357aa1abc60c01b3fbf8dacb2694.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/27e574eab03093d302f01e5ceb42d0af.jpg\" _src=\"http://yanxuan.nosdn.127.net/27e574eab03093d302f01e5ceb42d0af.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/30228bd984383c97633eef50ca556406.jpg\" _src=\"http://yanxuan.nosdn.127.net/30228bd984383c97633eef50ca556406.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/baa3cc805dc0afb4257c30466771535a.jpg\" _src=\"http://yanxuan.nosdn.127.net/baa3cc805dc0afb4257c30466771535a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/daa37937c3440919e597e4954e68f646.jpg\" _src=\"http://yanxuan.nosdn.127.net/daa37937c3440919e597e4954e68f646.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/82df87910187f081e2a4d5f5a06df4cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/82df87910187f081e2a4d5f5a06df4cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/eaa197c3d63c8479e38f46595df50a5e.jpg\" _src=\"http://yanxuan.nosdn.127.net/eaa197c3d63c8479e38f46595df50a5e.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/56cf9f1b8de8627ad0d064843d97cd96.jpg\" _src=\"http://yanxuan.nosdn.127.net/56cf9f1b8de8627ad0d064843d97cd96.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99ad88418c88c550b183dc12a9280a1d.jpg\" _src=\"http://yanxuan.nosdn.127.net/99ad88418c88c550b183dc12a9280a1d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a84aafb6ddbe25f32bddc4f843ad35d0.jpg\" _src=\"http://yanxuan.nosdn.127.net/a84aafb6ddbe25f32bddc4f843ad35d0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9ce402bfb9d08603259264e9115166b2.jpg\" _src=\"http://yanxuan.nosdn.127.net/9ce402bfb9d08603259264e9115166b2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1a7248d14d630770dfff1b17350219ba.jpg\" _src=\"http://yanxuan.nosdn.127.net/1a7248d14d630770dfff1b17350219ba.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/43113bc52b7eece12f777092d9b04c3f.jpg\" _src=\"http://yanxuan.nosdn.127.net/43113bc52b7eece12f777092d9b04c3f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/fbe65886e9405ceb1a43fb3097fd709a.jpg\" _src=\"http://yanxuan.nosdn.127.net/fbe65886e9405ceb1a43fb3097fd709a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e098163e428171418a77c077a8330299.jpg\" _src=\"http://yanxuan.nosdn.127.net/e098163e428171418a77c077a8330299.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/cbb9a88692c9621652244844bf0b299d.jpg\" _src=\"http://yanxuan.nosdn.127.net/cbb9a88692c9621652244844bf0b299d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7d8264c945ccb68d432dcaeb86e3e4ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/7d8264c945ccb68d432dcaeb86e3e4ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/5e0a467456d69bc746e6bd7797f6963b.jpg\" _src=\"http://yanxuan.nosdn.127.net/5e0a467456d69bc746e6bd7797f6963b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a58d0c630b0e2f51fa49aef8687a9e16.jpg\" _src=\"http://yanxuan.nosdn.127.net/a58d0c630b0e2f51fa49aef8687a9e16.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1de7c562962e54da6a63e749634eb008.jpg\" _src=\"http://yanxuan.nosdn.127.net/1de7c562962e54da6a63e749634eb008.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8931ee6e2b4b3ed3454184093b6471ed.jpg\" _src=\"http://yanxuan.nosdn.127.net/8931ee6e2b4b3ed3454184093b6471ed.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b032ca9815193ec258be3ffa0a25da3.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b032ca9815193ec258be3ffa0a25da3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/bfd12f882162e93008c97bff3187f694.jpg\" _src=\"http://yanxuan.nosdn.127.net/bfd12f882162e93008c97bff3187f694.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/79d69e15728310ec458ec665a287fc87.jpg\" _src=\"http://yanxuan.nosdn.127.net/79d69e15728310ec458ec665a287fc87.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e10b0c8d89689483eceea36aa330deb4.jpg\" _src=\"http://yanxuan.nosdn.127.net/e10b0c8d89689483eceea36aa330deb4.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88c5b10b0916839ae7cf6ca1b8c8d83f.jpg\" _src=\"http://yanxuan.nosdn.127.net/88c5b10b0916839ae7cf6ca1b8c8d83f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/17b3ace86142f2b8c7f29ed10d1dba55.jpg\" _src=\"http://yanxuan.nosdn.127.net/17b3ace86142f2b8c7f29ed10d1dba55.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83f9993c4dda4898693ba3fe9f313c1f.jpg\" _src=\"http://yanxuan.nosdn.127.net/83f9993c4dda4898693ba3fe9f313c1f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9310f4e403eb5db6107bfc280c3e6cf8.jpg\" _src=\"http://yanxuan.nosdn.127.net/9310f4e403eb5db6107bfc280c3e6cf8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7ba895b4d7507984a26344d7c03db550.jpg\" _src=\"http://yanxuan.nosdn.127.net/7ba895b4d7507984a26344d7c03db550.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/34f3faaad28a93f140f3f1b78def4bce.jpg\" _src=\"http://yanxuan.nosdn.127.net/34f3faaad28a93f140f3f1b78def4bce.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/355dc9d6e4a8a1a8561183641ef2890a.jpg\" _src=\"http://yanxuan.nosdn.127.net/355dc9d6e4a8a1a8561183641ef2890a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f2b6a2155e30bf99750756ec4fb99f11.jpg\" _src=\"http://yanxuan.nosdn.127.net/f2b6a2155e30bf99750756ec4fb99f11.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 29,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/6f162e1b98906c2a02c75b40ff9659d3.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/bda805b0a2464b6ec33c18981565e50e.png",
      "retail_price": 559,
      "sell_volume": 199,
      "primary_product_id": 1148176,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    },
    {
      "id": 1147048,
      "category_id": 1008002,
      "goods_sn": "1147048",
      "name": "简约知性系列居家地毯 蓝灰格",
      "brand_id": 0,
      "goods_number": 100,
      "keywords": "",
      "goods_brief": "沉稳双拼色 居家温柔伴护",
      "goods_desc": "<p><img src=\"http://yanxuan.nosdn.127.net/037e5909a5bec975c67bf61d193d7b72.jpg\" _src=\"http://yanxuan.nosdn.127.net/037e5909a5bec975c67bf61d193d7b72.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/88486bfa3d7bd68c7780df5cc01e7a7d.jpg\" _src=\"http://yanxuan.nosdn.127.net/88486bfa3d7bd68c7780df5cc01e7a7d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77c2d1819d99dde7cad8c140048a46aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/77c2d1819d99dde7cad8c140048a46aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f49aed0ebcd5c54f3edb8240921e3a46.jpg\" _src=\"http://yanxuan.nosdn.127.net/f49aed0ebcd5c54f3edb8240921e3a46.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60b923642f98ca62ca3d9a6fe0db8800.jpg\" _src=\"http://yanxuan.nosdn.127.net/60b923642f98ca62ca3d9a6fe0db8800.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/782d6edfc30d1a53711d5f0f6145f8fd.jpg\" _src=\"http://yanxuan.nosdn.127.net/782d6edfc30d1a53711d5f0f6145f8fd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3b10a5a5f29340056cb6b1673420f46c.jpg\" _src=\"http://yanxuan.nosdn.127.net/3b10a5a5f29340056cb6b1673420f46c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e2e721a8f26030ba31f0b290c47ba232.jpg\" _src=\"http://yanxuan.nosdn.127.net/e2e721a8f26030ba31f0b290c47ba232.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/77d18b39a7d8b603b869ca4cb8d7235b.jpg\" _src=\"http://yanxuan.nosdn.127.net/77d18b39a7d8b603b869ca4cb8d7235b.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/c266d8f75bc074531033430882a93d8a.jpg\" _src=\"http://yanxuan.nosdn.127.net/c266d8f75bc074531033430882a93d8a.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ceb7a59b3c56f7ced051cae61d70daf6.jpg\" _src=\"http://yanxuan.nosdn.127.net/ceb7a59b3c56f7ced051cae61d70daf6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0db841700c868c08d627f01c354b013c.jpg\" _src=\"http://yanxuan.nosdn.127.net/0db841700c868c08d627f01c354b013c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/008ea04b11a0f68116e5eb180ca8a6a0.jpg\" _src=\"http://yanxuan.nosdn.127.net/008ea04b11a0f68116e5eb180ca8a6a0.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/dfa3513280704216372dade1751b2bc6.jpg\" _src=\"http://yanxuan.nosdn.127.net/dfa3513280704216372dade1751b2bc6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1287987157d7a1767ccaec835bb82b17.jpg\" _src=\"http://yanxuan.nosdn.127.net/1287987157d7a1767ccaec835bb82b17.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/041f4c058fd201716c456d32588e0611.jpg\" _src=\"http://yanxuan.nosdn.127.net/041f4c058fd201716c456d32588e0611.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/22832d570b7eaf8153d5038d9095b990.jpg\" _src=\"http://yanxuan.nosdn.127.net/22832d570b7eaf8153d5038d9095b990.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e5651dedb8b4d5c1d40345f13a4ad622.jpg\" _src=\"http://yanxuan.nosdn.127.net/e5651dedb8b4d5c1d40345f13a4ad622.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/0b988f3146c079e488eeb05ba03cae37.jpg\" _src=\"http://yanxuan.nosdn.127.net/0b988f3146c079e488eeb05ba03cae37.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6d53d4374b9a800da1eb215b6215b403.jpg\" _src=\"http://yanxuan.nosdn.127.net/6d53d4374b9a800da1eb215b6215b403.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/1abd7dd665582e0eb1c8e4bd6196b6cb.jpg\" _src=\"http://yanxuan.nosdn.127.net/1abd7dd665582e0eb1c8e4bd6196b6cb.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/39561bb5901a7a80bf362bf4b7b96d30.jpg\" _src=\"http://yanxuan.nosdn.127.net/39561bb5901a7a80bf362bf4b7b96d30.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/99eff53c1440f72152c2b264c22244a7.jpg\" _src=\"http://yanxuan.nosdn.127.net/99eff53c1440f72152c2b264c22244a7.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8e54bd5c82506db1eed358edcdbd6ef8.jpg\" _src=\"http://yanxuan.nosdn.127.net/8e54bd5c82506db1eed358edcdbd6ef8.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/83ca52b41e1907932bc55330fd5a5cad.jpg\" _src=\"http://yanxuan.nosdn.127.net/83ca52b41e1907932bc55330fd5a5cad.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/6f58dc91de46bbf93fbf054de64958aa.jpg\" _src=\"http://yanxuan.nosdn.127.net/6f58dc91de46bbf93fbf054de64958aa.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/08d20c7dc0ae462a176ac52a58e7b297.jpg\" _src=\"http://yanxuan.nosdn.127.net/08d20c7dc0ae462a176ac52a58e7b297.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/ca1db2649c0a5c67ed319cb212332380.jpg\" _src=\"http://yanxuan.nosdn.127.net/ca1db2649c0a5c67ed319cb212332380.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2feac4d0a9ef0053863b81e37f7fe9fe.jpg\" _src=\"http://yanxuan.nosdn.127.net/2feac4d0a9ef0053863b81e37f7fe9fe.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b9d2fa42d4fec3abd1c151a8dbdab0ef.jpg\" _src=\"http://yanxuan.nosdn.127.net/b9d2fa42d4fec3abd1c151a8dbdab0ef.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/e78a8555da079fb963f78fc9149f93cd.jpg\" _src=\"http://yanxuan.nosdn.127.net/e78a8555da079fb963f78fc9149f93cd.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/b5384e883e1e96640d1adfca1c2e511f.jpg\" _src=\"http://yanxuan.nosdn.127.net/b5384e883e1e96640d1adfca1c2e511f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/9c8ec5307f7f0c5a3dcea9916bbbf091.jpg\" _src=\"http://yanxuan.nosdn.127.net/9c8ec5307f7f0c5a3dcea9916bbbf091.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/3c59d89c8b46e0e740fd6d8f40071422.jpg\" _src=\"http://yanxuan.nosdn.127.net/3c59d89c8b46e0e740fd6d8f40071422.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4f5640cac8b41175cf3fb620f25ed7ec.jpg\" _src=\"http://yanxuan.nosdn.127.net/4f5640cac8b41175cf3fb620f25ed7ec.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/20ab37f417610381659ad47de48aa42f.jpg\" _src=\"http://yanxuan.nosdn.127.net/20ab37f417610381659ad47de48aa42f.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/f676f5243a835cb63d76e20423666337.jpg\" _src=\"http://yanxuan.nosdn.127.net/f676f5243a835cb63d76e20423666337.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/8b9e1a348d1766c803f9b31221f94553.jpg\" _src=\"http://yanxuan.nosdn.127.net/8b9e1a348d1766c803f9b31221f94553.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/a49199ab0ee762df58a2dce4bd26b1e3.jpg\" _src=\"http://yanxuan.nosdn.127.net/a49199ab0ee762df58a2dce4bd26b1e3.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/4635e2b0daeca9d6dbaf66dc6a74b2f6.jpg\" _src=\"http://yanxuan.nosdn.127.net/4635e2b0daeca9d6dbaf66dc6a74b2f6.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/2d05ee8ffcca5df74090153c8892cb4d.jpg\" _src=\"http://yanxuan.nosdn.127.net/2d05ee8ffcca5df74090153c8892cb4d.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/60c532e803c2d4a75c3da1200797d29c.jpg\" _src=\"http://yanxuan.nosdn.127.net/60c532e803c2d4a75c3da1200797d29c.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/75b9feace19e5c3c2e5a9e8dca01a0f2.jpg\" _src=\"http://yanxuan.nosdn.127.net/75b9feace19e5c3c2e5a9e8dca01a0f2.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/7f5ef8ad3f27f9f6dd1826afe0494c29.jpg\" _src=\"http://yanxuan.nosdn.127.net/7f5ef8ad3f27f9f6dd1826afe0494c29.jpg\" style=\"\"/></p><p><img src=\"http://yanxuan.nosdn.127.net/50aab2e77e905e1f0c1a71ec25739207.jpg\" _src=\"http://yanxuan.nosdn.127.net/50aab2e77e905e1f0c1a71ec25739207.jpg\" style=\"\"/></p><p><br/></p>",
      "is_on_sale": 1,
      "add_time": 0,
      "sort_order": 30,
      "is_delete": 0,
      "attribute_category": 0,
      "counter_price": 0,
      "extra_price": 0,
      "is_new": 0,
      "goods_unit": "件",
      "primary_pic_url": "http://yanxuan.nosdn.127.net/3386744ee6833d13a6f6b843cb35f6c6.jpg",
      "list_pic_url": "http://yanxuan.nosdn.127.net/fd7920a2eadd10fa10c0c03959a2abe0.png",
      "retail_price": 559,
      "sell_volume": 183,
      "primary_product_id": 1148177,
      "unit_price": 0,
      "promotion_desc": "限时购",
      "promotion_tag": "",
      "app_exclusive_price": 0,
      "is_app_exclusive": 0,
      "is_limited": 0,
      "is_hot": 0
    }
  ],
  "collected": false,
  "allnumber": 2
}
```

### 获取专题列表

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/topic/listaction `

**请求方式：**

- GET 

**参数：** 

| 参数名  | 必选  | 类型  | 说明     |
|:---- |:--- |:--- | ------ |
| page | 是   | int | 当前请求页数 |

**返回示例**

```json
{
  "page": "1",
  "total": 4,
  "data": [
    {
      "id": 314,
      "title": "关爱他成长的每一个足迹",
      "price_info": 0,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14943267735961674.jpg",
      "subtitle": "专业运动品牌同厂，毛毛虫鞋买二送一"
    },
    {
      "id": 313,
      "title": "一次解决5个节日送礼难题",
      "price_info": 59.9,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14942996754171334.jpg",
      "subtitle": "这些就是他们想要的礼物清单"
    },
    {
      "id": 300,
      "title": "秒杀化学洗涤剂的纯天然皂",
      "price_info": 0,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14939843143621089.jpg",
      "subtitle": "前段时间有朋友跟我抱怨，和婆婆住到一起才发现生活理念有太多不和。别的不提，光是洗..."
    },
    {
      "id": 299,
      "title": "买过的人都说它是差旅神器",
      "price_info": 0,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14938873919030679.jpg",
      "subtitle": "许多人经历过旅途中内裤洗晾不便的烦恼，尤其与旅伴同居一室时，晾在卫生间里的内裤更..."
    },
    {
      "id": 295,
      "title": "他们在严选遇见的新生活",
      "price_info": 35.8,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14938092956370380.jpg",
      "subtitle": "多款商品直减中，最高直减400元"
    }
  ]
}
```

### 专题详情加下方四个专题推荐

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/topic/detailaction `

**请求方式：**

- GET 

**参数：** 

| 参数名 | 必选  | 类型  | 说明   |
|:--- |:--- |:--- | ---- |
| id  | 是   | int | 专题id |

**返回示例**

```json
{
  "data": {
    "id": 314,
    "title": "关爱他成长的每一个足迹",
    "content": "<img src=\"//yanxuan.nosdn.127.net/75c55a13fde5eb2bc2dd6813b4c565cc.jpg\">\n    <img src=\"//yanxuan.nosdn.127.net/e27e1de2b271a28a21c10213b9df7e95.jpg\">\n    <img src=\"//yanxuan.nosdn.127.net/9d413d1d28f753cb19096b533d53418d.jpg\">\n    <img src=\"//yanxuan.nosdn.127.net/64b0f2f350969e9818a3b6c43c217325.jpg\">\n    <img src=\"//yanxuan.nosdn.127.net/a668e6ae7f1fa45565c1eac221787570.jpg\">\n    <img src=\"//yanxuan.nosdn.127.net/0d4004e19728f2707f08f4be79bbc774.jpg\">\n    <img src=\"//yanxuan.nosdn.127.net/79ee021bbe97de7ecda691de6787241f.jpg\">",
    "avatar": "https://yanxuan.nosdn.127.net/14943186689221563.png",
    "item_pic_url": "https://yanxuan.nosdn.127.net/14943267735961674.jpg",
    "subtitle": "专业运动品牌同厂，毛毛虫鞋买二送一",
    "topic_category_id": 2,
    "price_info": 0,
    "read_count": "6.4k",
    "scene_pic_url": "https://yanxuan.nosdn.127.net/14943267735961674.jpg",
    "topic_template_id": 0,
    "topic_tag_id": 0,
    "sort_order": 1,
    "is_show": 1
  },
  "recommendList": [
    {
      "id": 314,
      "title": "关爱他成长的每一个足迹",
      "price_info": 0,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14943267735961674.jpg",
      "subtitle": "专业运动品牌同厂，毛毛虫鞋买二送一"
    },
    {
      "id": 313,
      "title": "一次解决5个节日送礼难题",
      "price_info": 59.9,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14942996754171334.jpg",
      "subtitle": "这些就是他们想要的礼物清单"
    },
    {
      "id": 300,
      "title": "秒杀化学洗涤剂的纯天然皂",
      "price_info": 0,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14939843143621089.jpg",
      "subtitle": "前段时间有朋友跟我抱怨，和婆婆住到一起才发现生活理念有太多不和。别的不提，光是洗..."
    },
    {
      "id": 299,
      "title": "买过的人都说它是差旅神器",
      "price_info": 0,
      "scene_pic_url": "https://yanxuan.nosdn.127.net/14938873919030679.jpg",
      "subtitle": "许多人经历过旅途中内裤洗晾不便的烦恼，尤其与旅伴同居一室时，晾在卫生间里的内裤更..."
    }
  ]
}
```

### 搜索关键词和搜索历史接口

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/search/indexaction `

**请求方式：**

- GET 

**参数：** 

| 参数名    | 必选  | 类型     | 说明     |
|:------ |:--- |:------ | ------ |
| openId | 是   | string | 微信唯一识别 |

**返回示例**

```json
{
  "defaultKeyword": {
    "keyword": "520元礼包抢先领",
    "is_hot": 1,
    "is_default": 1,
    "is_show": 1,
    "sort_order": 1,
    "scheme _url": "",
    "id": 1,
    "type": 0
  },
  "hotKeywordList": [
    {
      "keyword": "520元礼包抢先领",
      "is_hot": 1
    },
    {
      "keyword": "单鞋",
      "is_hot": 0
    },
    {
      "keyword": "墨镜",
      "is_hot": 0
    },
    {
      "keyword": "夏凉被",
      "is_hot": 0
    },
    {
      "keyword": "新品上市",
      "is_hot": 0
    },
    {
      "keyword": "日式",
      "is_hot": 0
    },
    {
      "keyword": "母亲节",
      "is_hot": 0
    }
  ],
  "historyData": []
}
```

### 关键词搜索提示

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/search/helperaction `

**请求方式：**

- GET 

**参数：** 

| 参数名     | 必选  | 类型     | 说明    |
|:------- |:--- |:------ | ----- |
| keyword | 是   | string | 搜索关键词 |

**返回示例**

```json
{
  "keywords": [
    {
      "id": 1009024,
      "name": "日式和风懒人沙发",
      "list_pic_url": "http://yanxuan.nosdn.127.net/149dfa87a7324e184c5526ead81de9ad.png",
      "retail_price": 599
    },
    {
      "id": 1109008,
      "name": "云端沙发组合",
      "list_pic_url": "http://yanxuan.nosdn.127.net/c5be2604c0e4186a4e7079feeb742cee.png",
      "retail_price": 3999
    }
  ]
}
```

### 搜索记录添加到数据库

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/search/addhistoryaction `

**请求方式：**

- POST 

**参数：** 

| 参数名     | 必选  | 类型     | 说明  |
|:------- |:--- |:------ | --- |
| keyword | 是   | String | 关键词 |
| openId  | 是   | string | 无   |

**返回示例**

```json
{
  "data": "success"
}
```

### 清空搜索记录

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/search/clearhistoryAction `

**请求方式：**

- POST 

**参数：** 

| 参数名    | 必选  | 类型     | 说明  |
|:------ |:--- |:------ | --- |
|        | 是   | string | 无   |
| openId | 是   | string | 无   |

**返回示例**

```json
{
  "data": "清除成功"
}
```

### 添加收藏或者移除收藏(相同的参数请求第二次代表移除收藏)

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/collect/addcollect `

**请求方式：**

- POST 

**参数：** 

| 参数名     | 必选  | 类型     | 说明   |
|:------- |:--- |:------ | ---- |
| goodsId | 是   | int    | 商品ID |
| openId  | 是   | string | 无    |

**返回示例**

```json
{
  "data": "success"
}
```

### 获取收藏列表

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/collect/listAction `

**请求方式：**

- GET 

**参数：** 

| 参数名    | 必选  | 类型     | 说明  |
|:------ |:--- |:------ | --- |
| openId | 是   | string | 无   |

**返回示例**

```json
{
  "collectGoodsList": [
    {
      "id": 1035006,
      "name": "全棉单面割绒浴室地垫",
      "list_pic_url": "http://yanxuan.nosdn.127.net/ee92704f3b8323905b51fc647823e6e5.png",
      "retail_price": 56,
      "goods_brief": "手工制作，纯棉材质，柔软舒适"
    }
  ]
}
```

### 添加商品进入购物车

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/cart/addCart `

**请求方式：**

- POST 

**参数：** 

| 参数名     | 必选  | 类型     | 说明   |
|:------- |:--- |:------ | ---- |
| goodsId | 是   | int    | 商品列表 |
| number  | 是   | int    | 商品数量 |
| openId  | 是   | string | 无    |

**返回示例**

```json
{
  "data": "success"
}
```

### 删除购物车商品

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/cart/deleteAction `

**请求方式：**

- GET 

**参数：** 

| 参数名 | 必选  | 类型  | 说明         |
|:--- |:--- |:--- | ---------- |
| id  | 是   | int | 商品在购物车列表id |

**返回示例**

```json
{
  "data": true
}
```

### 购物车商品列表

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/cart/cartList `

**请求方式：**

- GET 

**参数：** 

| 参数名    | 必选  | 类型     | 说明  |
|:------ |:--- |:------ | --- |
| openId | 是   | string | 无   |

**返回示例**

```json
{
  "data": [
    {
      "id": 130,
      "user_id": "oE43c4jeywabPOafcNu7Il83B3mY",
      "goods_id": 1134030,
      "goods_name": "简约知性记忆棉坐垫",
      "retail_price": 46,
      "number": 5,
      "list_pic_url": "http://yanxuan.nosdn.127.net/aa49dfe878becf768eddc4c1636643a6.png"
    }
  ]
}
```

### 提交订单

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/order/submitAction `

**请求方式：**

- POST 

**参数：** 

| 参数名      | 必选  | 类型     | 说明      |
|:-------- |:--- |:------ | ------- |
| allPrise | 是   | int    | 提交的商品总价 |
| goodsId  | 是   | int    | 商品id    |
| openId   | 是   | string | 无       |

**返回示例**

```json
{
  "data": true
}
```

### 获取订单详情

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/order/detailAction `

**请求方式：**

- GET 

**参数：** 

| 参数名       | 必选  | 类型     | 说明  |
|:--------- |:--- |:------ | --- |
| addressId | 是   | string | 无   |
| openId    | 是   | string | 无   |

**返回示例**

```json
{
  "allPrise": "758",
  "goodsList": [
    {
      "id": 125,
      "user_id": "oQmbb4sNZdxaUQZ0sfYgvtOP2S7c",
      "goods_id": 1006013,
      "goods_name": "双宫茧桑蚕丝被 空调被",
      "retail_price": 699,
      "number": 1,
      "list_pic_url": "http://yanxuan.nosdn.127.net/583812520c68ca7995b6fac4c67ae2c7.png"
    }
  ],
  "address": {
    "id": 33,
    "name": "科比",
    "user_id": "oQmbb4sNZdxaUQZ0sfYgvtOP2S7c",
    "address": "河北省 石家庄市 桥东区",
    "mobile": "123456789",
    "is_default": 1,
    "address_detail": "斯柯达副科级上刊登了附近路口"
  }
}
```

### 保存修改后的收货地址

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/address/saveAction `

**请求方式：**

- POST 

**参数：** 

| 参数名          | 必选  | 类型     | 说明          |
|:------------ |:--- |:------ | ----------- |
| openId       | 是   | string | 唯一标识        |
| address      | 是   | string | 省市区         |
| addressId    | 是   | int    | 地址id        |
| checked      | 是   | string | 是否是默认地址 （1） |
| detailadress | 是   | string | 详细地址        |
| telNumber    | 是   | int    | 电话          |
| userName     | 是   | string | 用户名         |

**返回示例**

```json
{
  "data": true
}
```

### 获取收货地址列表

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/address/getListAction `

**请求方式：**

- GET 

**参数：** 

| 参数名    | 必选  | 类型     | 说明  |
|:------ |:--- |:------ | --- |
| openId | 是   | string | 无   |

**返回示例**

```json
{
  "data": [
    {
      "id": 33,
      "name": "kebi",
      "user_id": "oQmbb4sNZdxaUQZ0sfYgvtOP2S7c",
      "address": "河北省 石家庄市 桥东区",
      "mobile": "123456789",
      "is_default": 1,
      "address_detail": "斯柯达副科级上刊登了附近路口"
    },
    {
      "id": 23,
      "name": "何玉硕",
      "user_id": "oQmbb4sNZdxaUQZ0sfYgvtOP2S7c",
      "address": "广东省 广州市 海珠区",
      "mobile": "020-81167888",
      "is_default": 0,
      "address_detail": "新港中路397号"
    }
  ]
}
```

### 获取收货地址详情数据

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/address/detailAction `

**请求方式：**

- GET 

**参数：** 

| 参数名 | 必选  | 类型  | 说明   |
|:--- |:--- |:--- | ---- |
| id  | 是   | int | 地址id |

**返回示例**

```json
{
  "data": {
    "id": 33,
    "name": "kebi",
    "user_id": "oQmbb4sNZdxaUQZ0sfYgvtOP2S7c",
    "address": "河北省 石家庄市 桥东区",
    "mobile": "123456789",
    "is_default": 1,
    "address_detail": "斯柯达副科级上刊登了附近路口"
  }
}
```

### 删除收货地址

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/address/deleteAction `

**请求方式：**

- GET 

**参数：** 

| 参数名 | 必选  | 类型  | 说明     |
|:--- |:--- |:--- | ------ |
| id  | 是   | int | 收货地址id |

**返回示例**

```json
{
  "data": true
}
```

### 意见反馈

**请求URL：** 

- ` https://shop.yangxiansheng.top/heyushuo/feedback/submitAction `

**请求方式：**

- POST 

**参数：** 

| 参数名     | 必选  | 类型     | 说明    |
|:------- |:--- |:------ | ----- |
| content | 是   | int    | 无     |
| openId  | 是   | string | 无     |
| name    | 是   | string | 微信用户名 |
| phone   | 是   | int    | 电话    |

**返回示例**

```json
{
  "data": true
}
```
