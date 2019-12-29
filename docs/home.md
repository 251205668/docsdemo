# 豆瓣电影 API Doc

## 说明

V2版API权限分3类:

- 公开（对应Required Scope URI ：movie_basic_r, movie_basic_w）- 所有开发者均可申请，审核通过。限定40次请求/分钟。开放基本数据接口，一般的个人爱好者自建网站或应用都会满足。

- 高级（对应Required Scope URI ：movie_advance_r, movie_advance_w） - 在运行过一段时间之后，如果这个非商业网站（例如非盈利性质的图书馆，学校，公益组织等）的确出众，且价值观符合Douban，无版权问题，又不和豆瓣电影有正面的商业竞争，可以申请高级权限。开放基本上所有的接口。

- 商务（对应Required Scope URI ：movie_premium_r, movie_premium_w）- 应用于商务合作，不限制次数，开放有限接口。已经商业化网站请使用此接口。 移植到V2之后，只要满足我们的API规定要求（见后），即可开通。


附：`apikey`:`0b2bdeda43b5688921839c8ecb20399b`

## Api列表

### 正在热映

url：`https://api.douban.com/v2/movie/in_theaters`

拼接参数：

- `apikey`：apikey
- `city`：所在城市，例如`北京`、`上海`等
- `count`：返回数量(该值不变)
- `start`：从第多少个开始
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/in_theaters?apikey=0b2bdeda43b5688921839c8ecb20399b&city=北京&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/in_theaters?apikey=0b2bdeda43b5688921839c8ecb20399b&city=北京&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/in_theaters?apikey=0b2bdeda43b5688921839c8ecb20399b&city=北京&start=0&count=20`](https://api.douban.com/v2/movie/in_theaters?apikey=0b2bdeda43b5688921839c8ecb20399b&city=北京&start=0&count=20)

json 示例：

```js
{
	"count": 2,
	"start": 0,
	"total": 27,
	"subjects": [{
		"rating": {
			"max": 10,
			"average": 7.3,
			"details": {
				"1": 376,
				"2": 1475,
				"3": 7846,
				"4": 11788,
				"5": 3652
			},
			"stars": "40",
			"min": 0
		},
		"genres": [
			"剧情",
			"喜剧"
		],
		"title": "一出好戏",
		"casts": [{
				"avatars": {
					"small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
					"large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
					"medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp"
				},
				"name_en": "Bo Huang",
				"name": "黄渤",
				"alt": "https://movie.douban.com/celebrity/1274242/",
				"id": "1274242"
			}
		],
		"durations": [
			"134分钟"
		],
		"collect_count": 257967,
		"mainland_pubdate": "2018-08-10",
		"has_video": false,
		"original_title": "一出好戏",
		"subtype": "movie",
		"directors": [{
			"avatars": {
				"small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
				"large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
				"medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp"
			},
			"name_en": "Bo Huang",
			"name": "黄渤",
			"alt": "https://movie.douban.com/celebrity/1274242/",
			"id": "1274242"
		}],
		"pubdates": [
			"2018-08-10(中国大陆)"
		],
		"year": "2018",
		"images": {
			"small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2529571873.webp",
			"large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2529571873.webp",
			"medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2529571873.webp"
		},
		"alt": "https://movie.douban.com/subject/26985127/",
		"id": "26985127"
	}],
	"title": "正在上映的电影-北京"
}
```


字段解析：

- `count`：返回条数
- `start`：返回条数开始计数
- `total`：总条数
- `subjects`：正在上映的电影信息，属性解析[见附录](#subject_attr)
- `title`：标头


### 搜索电影

url：`https://api.douban.com/v2/movie/search `

拼接参数：

- `apikey`：apikey
- `q`：查询关键字，例如`霸王别姬`、`张艺谋`等。与`tag`二选一
- `tag`：标签，例如`青春`、`喜剧`等。与`q`二选一
- `count`：返回数量
- `start`：从第多少个开始
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/search?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd&q=霸王别姬`](https://api.douban.com/v2/movie/search?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd&q=霸王别姬) 
或 
[`https://api.douban.com/v2/movie/search?apikey=0b2bdeda43b5688921839c8ecb20399b&tag=喜剧&start=0&count=20`](https://api.douban.com/v2/movie/search?apikey=0b2bdeda43b5688921839c8ecb20399b&tag=喜剧&start=0&count=20)

json 示例：

```js
{
	"count": 2,
	"start": 0,
	"total": 106,
	"subjects": [{
		"rating": {
			"max": 10,
			"average": 8.3,
			"details": {
				"1": 915,
				"2": 3924,
				"3": 43740,
				"4": 120115,
				"5": 92066
			},
			"stars": "45",
			"min": 0
		},
		"genres": [
			"喜剧",
			"犯罪"
		],
		"title": "疯狂的石头",
		"casts": [{
				"avatars": {
					"small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1505398270.58.webp",
					"large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1505398270.58.webp",
					"medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1505398270.58.webp"
				},
				"name_en": "Tao Guo",
				"name": "郭涛",
				"alt": "https://movie.douban.com/celebrity/1274274/",
				"id": "1274274"
			}
		],
		"durations": [
			"106 分钟(香港)",
			"98 分钟(中国大陆)"
		],
		"collect_count": 465490,
		"mainland_pubdate": "2006-06-30",
		"has_video": false,
		"original_title": "疯狂的石头",
		"subtype": "movie",
		"directors": [{
			"avatars": {
				"small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1366357991.6.webp",
				"large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1366357991.6.webp",
				"medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1366357991.6.webp"
			},
			"name_en": "Hao Ning",
			"name": "宁浩",
			"alt": "https://movie.douban.com/celebrity/1274265/",
			"id": "1274265"
		}],
		"pubdates": [
			"2006-06-30(中国大陆)",
			"2006-08-10(香港)"
		],
		"year": "2006",
		"images": {
			"small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p712241453.webp",
			"large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p712241453.webp",
			"medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p712241453.webp"
		},
		"alt": "https://movie.douban.com/subject/1862151/",
		"id": "1862151"
	}],
	"title": "搜索 \"黄渤\" 的结果"
}
```


字段解析：

- `count`：返回条数
- `start`：返回条数开始计数
- `total`：总条数
- `subjects`：搜索 "黄渤" 的结果的电影信息，属性解析[见附录](#subject_attr)
- `title`：标头


### 即将上映

url：`https://api.douban.com/v2/movie/coming_soon `

拼接参数：

- `apikey`：apikey
- `count`：返回数量
- `start`：从第多少个开始
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/coming_soon?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/coming_soon?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/coming_soon?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20`](https://api.douban.com/v2/movie/coming_soon?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20)

json 示例：

```js
{
	"count": 2,
	"start": 0,
	"total": 124,
	"subjects": [{
		"rating": {
			"max": 10,
			"average": 0,
			"details": {
				"1": 0,
				"2": 0,
				"3": 0,
				"4": 0,
				"5": 0
			},
			"stars": "00",
			"min": 0
		},
		"genres": [
			"喜剧",
			"奇幻"
		],
		"title": "快把我哥带走",
		"casts": [{
				"avatars": {
					"small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1465826349.1.webp",
					"large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1465826349.1.webp",
					"medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1465826349.1.webp"
				},
				"name_en": "Zifeng Zhang",
				"name": "张子枫",
				"alt": "https://movie.douban.com/celebrity/1274254/",
				"id": "1274254"
			}
		],
		"durations": [
			"115分钟"
		],
		"collect_count": 5494,
		"mainland_pubdate": "2018-08-17",
		"has_video": false,
		"original_title": "快把我哥带走",
		"subtype": "movie",
		"directors": [{
			"avatars": {
				"small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p13508.webp",
				"large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p13508.webp",
				"medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p13508.webp"
			},
			"name_en": "Fenfen Cheng",
			"name": "郑芬芬",
			"alt": "https://movie.douban.com/celebrity/1276077/",
			"id": "1276077"
		}],
		"pubdates": [
			"2018-08-17(中国大陆)"
		],
		"year": "2018",
		"images": {
			"small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2531080870.webp",
			"large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2531080870.webp",
			"medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2531080870.webp"
		},
		"alt": "https://movie.douban.com/subject/30122633/",
		"id": "30122633"
	}],
	"title": "即将上映的电影"
}
```


字段解析：

- `count`：返回条数
- `start`：返回条数开始计数
- `total`：总条数
- `subjects`：即将上映的电影信息，属性解析[见附录](#subject_attr)
- `title`：标头


### 新片榜

url：`https://api.douban.com/v2/movie/new_movies `

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/new_movies?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/new_movies?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/new_movies?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/new_movies?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：
```js

	{
	    "subjects": [
	        {
	            "rating": {
	                "max": 10,
	                "average": 7.5,
	                "details": {
	                    "1": 103,
	                    "2": 743,
	                    "3": 6257,
	                    "4": 8867,
	                    "5": 3584
	                },
	                "stars": "40",
	                "min": 0
	            },
	            "genres": [
	                "喜剧",
	                "动作",
	                "科幻"
	            ],
	            "title": "死侍2",
	            "casts": [
	                {
	                    "avatars": {
	                        "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p8515.webp",
	                        "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p8515.webp",
	                        "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p8515.webp"
	                    },
	                    "name_en": "Morena Baccarin",
	                    "name": "莫蕾娜·巴卡林",
	                    "alt": "https://movie.douban.com/celebrity/1017908/",
	                    "id": "1017908"
	                }
	            ],
	            "durations": [
	                "119分钟",
	                "134分钟(蓝光版)"
	            ],
	            "collect_count": 80758,
	            "mainland_pubdate": "",
	            "has_video": false,
	            "original_title": "Deadpool 2",
	            "subtype": "movie",
	            "directors": [
	                {
	                    "avatars": {
	                        "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1416221591.26.webp",
	                        "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1416221591.26.webp",
	                        "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1416221591.26.webp"
	                    },
	                    "name_en": "David Leitch",
	                    "name": "大卫·雷奇",
	                    "alt": "https://movie.douban.com/celebrity/1289765/",
	                    "id": "1289765"
	                }
	            ],
	            "pubdates": [
	                "2018-05-18(美国)"
	            ],
	            "year": "2018",
	            "images": {
	                "small": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2521499639.webp",
	                "large": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2521499639.webp",
	                "medium": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2521499639.webp"
	            },
	            "alt": "https://movie.douban.com/subject/26588308/",
	            "id": "26588308"
	        }
	    ],
	    "title": "豆瓣电影新片榜"
	}

```
字段解析：

- `subjects`：豆瓣电影新片榜电影信息，属性解析[见附录](#subject_attr)
- `title`：标头


### 口碑榜

url：`https://api.douban.com/v2/movie/weekly `

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/weekly?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/weekly?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/weekly?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/weekly?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：
```js

	{
	    "subjects": [
	        {
	            "subject": {
	                "rating": {
	                    "max": 10,
	                    "average": 8.7,
	                    "details": {
	                        "1": 73,
	                        "2": 215,
	                        "3": 3246,
	                        "4": 17571,
	                        "5": 18492
	                    },
	                    "stars": "45",
	                    "min": 0
	                },
	                "genres": [
	                    "剧情",
	                    "犯罪",
	                    "家庭"
	                ],
	                "title": "小偷家族",
	                "casts": [
	                    {
	                        "avatars": {
	                            "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1428591465.76.webp",
	                            "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1428591465.76.webp",
	                            "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1428591465.76.webp"
	                        },
	                        "name_en": "Mayu Matsuoka",
	                        "name": "松冈茉优",
	                        "alt": "https://movie.douban.com/celebrity/1320978/",
	                        "id": "1320978"
	                    }
	                ],
	                "durations": [
	                    "117分钟(中国大陆)",
	                    "121分钟"
	                ],
	                "collect_count": 200981,
	                "mainland_pubdate": "2018-08-03",
	                "has_video": false,
	                "original_title": "万引き家族",
	                "subtype": "movie",
	                "directors": [
	                    {
	                        "avatars": {
	                            "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1363134033.35.webp",
	                            "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1363134033.35.webp",
	                            "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1363134033.35.webp"
	                        },
	                        "name_en": "Hirokazu Koreeda",
	                        "name": "是枝裕和",
	                        "alt": "https://movie.douban.com/celebrity/1274351/",
	                        "id": "1274351"
	                    }
	                ],
	                "pubdates": [
	                    "2018-05-13(戛纳电影节)",
	                    "2018-06-08(日本)",
	                    "2018-08-03(中国大陆)"
	                ],
	                "year": "2018",
	                "images": {
	                    "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2530599636.webp",
	                    "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2530599636.webp",
	                    "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2530599636.webp"
	                },
	                "alt": "https://movie.douban.com/subject/27622447/",
	                "id": "27622447"
	            },
	            "rank": 1,
	            "delta": 0
	        }
	    ],
	    "title": "豆瓣电影本周口碑榜"
	}
```

字段解析：

- `subjects`：豆瓣电影本周口碑榜信息，weekly条目列表属性解析[见附录](#weekly_subject)
	- `subject`：影片信息，属性解析[见附录](#subject_attr)
- `title`：标头

### Top250

url：`https://api.douban.com/v2/movie/top250`

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空
- `count`：返回数量
- `start`：从第多少个开始

url 示例：
[`https://api.douban.com/v2/movie/top250?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=100&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/top250?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=100&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/top250?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=100`](https://api.douban.com/v2/movie/top250?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=100)

json 示例：
```js
	{
	    "count": 2,
	    "start": 0,
	    "total": 250,
	    "subjects": [
	        {
	            "rating": {
	                "max": 10,
	                "average": 9.6,
	                "details": {
	                    "1": 759,
	                    "2": 807,
	                    "3": 13506,
	                    "4": 113180,
	                    "5": 633410
	                },
	                "stars": "50",
	                "min": 0
	            },
	            "genres": [
	                "犯罪",
	                "剧情"
	            ],
	            "title": "肖申克的救赎",
	            "casts": [
	                {
	                    "avatars": {
	                        "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p17525.webp",
	                        "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p17525.webp",
	                        "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p17525.webp"
	                    },
	                    "name_en": "Tim Robbins",
	                    "name": "蒂姆·罗宾斯",
	                    "alt": "https://movie.douban.com/celebrity/1054521/",
	                    "id": "1054521"
	                }
	            ],
	            "durations": [
	                "142分钟"
	            ],
	            "collect_count": 1386741,
	            "mainland_pubdate": "",
	            "has_video": true,
	            "original_title": "The Shawshank Redemption",
	            "subtype": "movie",
	            "directors": [
	                {
	                    "avatars": {
	                        "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p230.webp",
	                        "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p230.webp",
	                        "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p230.webp"
	                    },
	                    "name_en": "Frank Darabont",
	                    "name": "弗兰克·德拉邦特",
	                    "alt": "https://movie.douban.com/celebrity/1047973/",
	                    "id": "1047973"
	                }
	            ],
	            "pubdates": [
	                "1994-09-10(多伦多电影节)",
	                "1994-10-14(美国)"
	            ],
	            "year": "1994",
	            "images": {
	                "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p480747492.webp",
	                "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p480747492.webp",
	                "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p480747492.webp"
	            },
	            "alt": "https://movie.douban.com/subject/1292052/",
	            "id": "1292052"
	        },
	        {
	            "rating": {
	                "max": 10,
	                "average": 9.5,
	                "details": {
	                    "1": 723,
	                    "2": 970,
	                    "3": 14431,
	                    "4": 98755,
	                    "5": 473795
	                },
	                "stars": "50",
	                "min": 0
	            },
	            "genres": [
	                "剧情",
	                "爱情",
	                "同性"
	            ],
	            "title": "霸王别姬",
	            "casts": [
	                {
	                    "avatars": {
	                        "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p67.webp",
	                        "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p67.webp",
	                        "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p67.webp"
	                    },
	                    "name_en": "Leslie Cheung",
	                    "name": "张国荣",
	                    "alt": "https://movie.douban.com/celebrity/1003494/",
	                    "id": "1003494"
	                }
	            ],
	            "durations": [
	                "171 分钟"
	            ],
	            "collect_count": 1015394,
	            "mainland_pubdate": "",
	            "has_video": true,
	            "original_title": "霸王别姬",
	            "subtype": "movie",
	            "directors": [
	                {
	                    "avatars": {
	                        "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1451727734.81.webp",
	                        "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1451727734.81.webp",
	                        "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1451727734.81.webp"
	                    },
	                    "name_en": "Kaige Chen",
	                    "name": "陈凯歌",
	                    "alt": "https://movie.douban.com/celebrity/1023040/",
	                    "id": "1023040"
	                }
	            ],
	            "pubdates": [
	                "1993-01-01(香港)"
	            ],
	            "year": "1993",
	            "images": {
	                "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p1910813120.webp",
	                "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p1910813120.webp",
	                "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p1910813120.webp"
	            },
	            "alt": "https://movie.douban.com/subject/1291546/",
	            "id": "1291546"
	        }
	    ],
	    "title": "豆瓣电影Top250"
	}
```
### 北美票房榜

url：`https://api.douban.com/v2/movie/us_box`

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/us_box?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/us_box?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd) 
或
[`https://api.douban.com/v2/movie/us_box?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/us_box?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：
```js

	{
	    "date": "8月10日 - 8月12日",
	    "subjects": [
	        {
	            "box": 44500000,
	            "new": true,
	            "rank": 1,
	            "subject": {
	                "rating": {
	                    "max": 10,
	                    "average": 6.1,
	                    "details": {
	                        "1": 207,
	                        "2": 1105,
	                        "3": 3632,
	                        "4": 1266,
	                        "5": 245
	                    },
	                    "stars": "30",
	                    "min": 0
	                },
	                "genres": [
	                    "动作",
	                    "科幻",
	                    "惊悚"
	                ],
	                "title": "巨齿鲨",
	                "casts": [
	                    {
	                        "avatars": {
	                            "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p424.webp",
	                            "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p424.webp",
	                            "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p424.webp"
	                        },
	                        "name_en": "Jason Statham",
	                        "name": "杰森·斯坦森",
	                        "alt": "https://movie.douban.com/celebrity/1049484/",
	                        "id": "1049484"
	                    }
	                ],
	                "durations": [
	                    "115分钟(中国大陆)",
	                    "113分钟"
	                ],
	                "collect_count": 60315,
	                "mainland_pubdate": "2018-08-10",
	                "has_video": false,
	                "original_title": "The Meg",
	                "subtype": "movie",
	                "directors": [
	                    {
	                        "avatars": {
	                            "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1379831737.28.webp",
	                            "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1379831737.28.webp",
	                            "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1379831737.28.webp"
	                        },
	                        "name_en": "Jon Turteltaub",
	                        "name": "乔·德特杜巴",
	                        "alt": "https://movie.douban.com/celebrity/1022710/",
	                        "id": "1022710"
	                    }
	                ],
	                "pubdates": [
	                    "2018-08-10(美国)",
	                    "2018-08-10(中国大陆)"
	                ],
	                "year": "2018",
	                "images": {
	                    "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2530572643.webp",
	                    "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2530572643.webp",
	                    "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2530572643.webp"
	                },
	                "alt": "https://movie.douban.com/subject/26426194/",
	                "id": "26426194"
	            }
	        },
	        {
	            "box": 20000000,
	            "new": false,
	            "rank": 2,
	            "subject": {
	                "rating": {
	                    "max": 10,
	                    "average": 8.1,
	                    "details": {
	                        "1": 7,
	                        "2": 56,
	                        "3": 512,
	                        "4": 1505,
	                        "5": 787
	                    },
	                    "stars": "40",
	                    "min": 0
	                },
	                "genres": [
	                    "动作",
	                    "惊悚",
	                    "冒险"
	                ],
	                "title": "碟中谍6：全面瓦解",
	                "casts": [
	                    {
	                        "avatars": {
	                            "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p567.webp",
	                            "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p567.webp",
	                            "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p567.webp"
	                        },
	                        "name_en": "Tom Cruise",
	                        "name": "汤姆·克鲁斯",
	                        "alt": "https://movie.douban.com/celebrity/1054435/",
	                        "id": "1054435"
	                    }
	                ],
	                "durations": [
	                    "147分钟",
	                    "148分钟(中国大陆)"
	                ],
	                "collect_count": 8286,
	                "mainland_pubdate": "2018-08-31",
	                "has_video": false,
	                "original_title": "Mission: Impossible - Fallout",
	                "subtype": "movie",
	                "directors": [
	                    {
	                        "avatars": {
	                            "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p52867.webp",
	                            "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p52867.webp",
	                            "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p52867.webp"
	                        },
	                        "name_en": "Christopher McQuarrie",
	                        "name": "克里斯托弗·麦奎里",
	                        "alt": "https://movie.douban.com/celebrity/1276314/",
	                        "id": "1276314"
	                    }
	                ],
	                "pubdates": [
	                    "2018-07-27(美国)",
	                    "2018-08-31(中国大陆)"
	                ],
	                "year": "2018",
	                "images": {
	                    "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2529365085.webp",
	                    "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2529365085.webp",
	                    "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2529365085.webp"
	                },
	                "alt": "https://movie.douban.com/subject/26336252/",
	                "id": "26336252"
	            }
	        }
	    ],
	    "title": "豆瓣电影北美票房榜"
	}
```

### 电影介绍

url：`http://api.douban.com/v2/movie/subject/{id}`

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`http://api.douban.com/v2/movie/subject/26985127?apikey=0b2bdeda43b5688921839c8ecb20399b&client=something&udid=dddddddddddddddddddddd`](http://api.douban.com/v2/movie/subject/26985127?apikey=0b2bdeda43b5688921839c8ecb20399b&client=something&udid=dddddddddddddddddddddd) 
或 
[`http://api.douban.com/v2/movie/subject/26985127?apikey=0b2bdeda43b5688921839c8ecb20399b`](http://api.douban.com/v2/movie/subject/26985127?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：

```js
	{
	    "rating": {
	        "max": 10,
	        "average": 7.3,
	        "details": {
	            "1": 400,
	            "2": 1559,
	            "3": 8372,
	            "4": 12422,
	            "5": 3830
	        },
	        "stars": "40",
	        "min": 0
	    },
	    "reviews_count": 3928,
	    "videos": [],
	    "wish_count": 327819,
	    "original_title": "一出好戏",
	    "blooper_urls": [
	        "http://vt1.doubanio.com/201808171748/5387fa64f769acfd4bb469b2d8c1cbbf/view/movie/M/302350039.mp4",
	        "http://vt1.doubanio.com/201808171748/a81797d3adf0c720e8b2c81c42dfb847/view/movie/M/302340882.mp4",
	        "http://vt1.doubanio.com/201808171748/3b269066fb68fb3cee38d6ab1629cb79/view/movie/M/302340704.mp4",
	        "http://vt1.doubanio.com/201808171748/1891c5706eeddacbefe8472af538648f/view/movie/M/302340334.mp4"
	    ],
	    "collect_count": 289629,
	    "images": {
	        "small": "http://img7.doubanio.com/view/photo/s_ratio_poster/public/p2529571873.webp",
	        "large": "http://img7.doubanio.com/view/photo/s_ratio_poster/public/p2529571873.webp",
	        "medium": "http://img7.doubanio.com/view/photo/s_ratio_poster/public/p2529571873.webp"
	    },
	    "douban_site": "",
	    "year": "2018",
	    "popular_comments": [
	        {
	            "rating": {
	                "max": 5,
	                "value": 4,
	                "min": 0
	            },
	            "useful_count": 2039,
	            "author": {
	                "uid": "estellalxy",
	                "avatar": "http://img7.doubanio.com/icon/u3004462-11.jpg",
	                "signature": "感觉已经有一座图书馆了",
	                "alt": "http://www.douban.com/people/estellalxy/",
	                "id": "3004462",
	                "name": "超新星芋圆兔"
	            },
	            "subject_id": "26985127",
	            "content": "ume的见面会。黄渤本人比电影里好看多了。电影本身不错，情节设置很好，就是开头的地方拍的有些粗糙，到岛上之后就开始精彩了。张艺兴的表演有突破。看宣传片以为电影要凉，结果居然意外的好看。推荐~",
	            "created_at": "2018-08-03 21:44:02",
	            "id": "1404127319"
	        }
	    ],
	    "alt": "https://movie.douban.com/subject/26985127/",
	    "id": "26985127",
	    "mobile_url": "https://movie.douban.com/subject/26985127/mobile",
	    "photos_count": 487,
	    "pubdate": "2018-08-10",
	    "title": "一出好戏",
	    "do_count": null,
	    "has_video": false,
	    "share_url": "http://m.douban.com/movie/subject/26985127",
	    "seasons_count": null,
	    "languages": [
	        "汉语普通话"
	    ],
	    "schedule_url": "https://movie.douban.com/subject/26985127/cinema/",
	    "writers": [
	        {
	            "avatars": {
	                "small": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
	                "large": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
	                "medium": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp"
	            },
	            "name_en": "Bo Huang",
	            "name": "黄渤",
	            "alt": "https://movie.douban.com/celebrity/1274242/",
	            "id": "1274242"
	        }
	    ],
	    "pubdates": [
	        "2018-08-10(中国大陆)"
	    ],
	    "website": "",
	    "tags": [
	        "人性",
	        "黑色幽默",
	        "荒岛求生",
	        "中国大陆",
	        "喜剧"
	    ],
	    "has_schedule": true,
	    "durations": [
	        "134分钟"
	    ],
	    "genres": [
	        "剧情",
	        "喜剧"
	    ],
	    "collection": null,
	    "trailers": [
	        {
	            "medium": "http://img3.doubanio.com/img/trailer/medium/2530290917.jpg?1533620442",
	            "title": "预告片：终极版 (中文字幕)",
	            "subject_id": "26985127",
	            "alt": "https://movie.douban.com/trailer/234740/",
	            "small": "http://img3.doubanio.com/img/trailer/small/2530290917.jpg?1533620442",
	            "resource_url": "http://vt1.doubanio.com/201808171748/f9604002151b9fe592e0d4f977590205/view/movie/M/302340740.mp4",
	            "id": "234740"
	        }
	    ],
	    "episodes_count": null,
	    "trailer_urls": [
	        "http://vt1.doubanio.com/201808171748/f9604002151b9fe592e0d4f977590205/view/movie/M/302340740.mp4",
	        "http://vt1.doubanio.com/201808171748/ca34bd06174fb1f9a8b5b07c6f209b34/view/movie/M/302340478.mp4",
	        "http://vt1.doubanio.com/201808171748/0307182b44b57f5ad6671b8c0c8f0f5e/view/movie/M/302330570.mp4",
	        "http://vt1.doubanio.com/201808171748/afd79d4cfc86f23719522c6c09ebe9b8/view/movie/M/302300863.mp4"
	    ],
	    "has_ticket": true,
	    "bloopers": [
	        {
	            "medium": "http://img3.doubanio.com/img/trailer/medium/2531101737.jpg?1534318330",
	            "title": "花絮：角色特辑 (中文字幕)",
	            "subject_id": "26985127",
	            "alt": "https://movie.douban.com/trailer/235039/",
	            "small": "http://img3.doubanio.com/img/trailer/small/2531101737.jpg?1534318330",
	            "resource_url": "http://vt1.doubanio.com/201808171748/5387fa64f769acfd4bb469b2d8c1cbbf/view/movie/M/302350039.mp4",
	            "id": "235039"
	        }
	    ],
	    "clip_urls": [
	        "http://vt1.doubanio.com/201808171748/a5e38ad610e94a59694fa2f10b55dfea/view/movie/M/302350004.mp4"
	    ],
	    "current_season": null,
	    "casts": [
	        {
	            "avatars": {
	                "small": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
	                "large": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
	                "medium": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp"
	            },
	            "name_en": "Bo Huang",
	            "name": "黄渤",
	            "alt": "https://movie.douban.com/celebrity/1274242/",
	            "id": "1274242"
	        }
	    ],
	    "countries": [
	        "中国大陆"
	    ],
	    "mainland_pubdate": "2018-08-10",
	    "photos": [
	        {
	            "thumb": "http://img3.doubanio.com/view/photo/m/public/p2531089766.webp",
	            "image": "http://img3.doubanio.com/view/photo/l/public/p2531089766.webp",
	            "cover": "http://img3.doubanio.com/view/photo/sqs/public/p2531089766.webp",
	            "alt": "https://movie.douban.com/photos/photo/2531089766/",
	            "id": "2531089766",
	            "icon": "http://img3.doubanio.com/view/photo/s/public/p2531089766.webp"
	        }
	    ],
	    "summary": "马进欠下债务，与远房表弟小兴在底层社会摸爬滚打，习惯性的买彩票，企图一夜暴富，并迎娶自己的同事姗姗。一日，公司全体员工出海团建，途中，马进收到了彩票中头奖的信息，六千万！就在马进狂喜自己翻身的日子终于到来之际，一场突如其来的滔天巨浪打破了一切。苏醒过来的众人发现身处荒岛 ，丧失了一切与外界的联系……",
	    "clips": [
	        {
	            "medium": "http://img7.doubanio.com/img/trailer/medium/2531084615.jpg?1534320094",
	            "title": "片段：片尾彩蛋 (中文字幕)",
	            "subject_id": "26985127",
	            "alt": "https://movie.douban.com/trailer/235004/",
	            "small": "http://img7.doubanio.com/img/trailer/small/2531084615.jpg?1534320094",
	            "resource_url": "http://vt1.doubanio.com/201808171748/a5e38ad610e94a59694fa2f10b55dfea/view/movie/M/302350004.mp4",
	            "id": "235004"
	        }
	    ],
	    "subtype": "movie",
	    "directors": [
	        {
	            "avatars": {
	                "small": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
	                "large": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp",
	                "medium": "http://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1656.webp"
	            },
	            "name_en": "Bo Huang",
	            "name": "黄渤",
	            "alt": "https://movie.douban.com/celebrity/1274242/",
	            "id": "1274242"
	        }
	    ],
	    "comments_count": 79479,
	    "popular_reviews": [
	        {
	            "rating": {
	                "max": 5,
	                "value": 4,
	                "min": 0
	            },
	            "title": "简明人类发展简史：如何解读这套乌托邦寓言？",
	            "subject_id": "26985127",
	            "author": {
	                "uid": "dreamfox",
	                "avatar": "http://img7.doubanio.com/icon/u2297669-12.jpg",
	                "signature": "公众号：dreamcrowfilm",
	                "alt": "http://www.douban.com/people/dreamfox/",
	                "id": "2297669",
	                "name": "乌鸦火堂"
	            },
	            "summary": "黄渤的《一出好戏》的故事内容，很容易让人联想起诺贝尔文学奖获得者威廉·戈尔丁的名作《蝇王》，但本片跟后者其实是相反的，包括角色设定、故事的发展脉络，人性的主题等等，用一句时髦形容词，《一出好戏》是...",
	            "alt": "https://movie.douban.com/review/9575824/",
	            "id": "9575824"
	        },
	        {
	            "rating": {
	                "max": 5,
	                "value": 4,
	                "min": 0
	            },
	            "title": "相信这确实是黄渤自己亲自导演的片子",
	            "subject_id": "26985127",
	            "author": {
	                "uid": "bixiongzz",
	                "avatar": "http://img7.doubanio.com/icon/u49422504-21.jpg",
	                "signature": "比熊贼贼改名了",
	                "alt": "http://www.douban.com/people/bixiongzz/",
	                "id": "49422504",
	                "name": "迷宝"
	            },
	            "summary": "1. 一直听说演员转型导演一般都只是挂名，并不是亲自操刀，那个挂名副导演的人才是在片场上起决定性作用的人。 从《泰囧》到《唐人街探案》，或者《煎饼侠》之类，其实都给我这种感觉，因为这些电影都是太圆润的...",
	            "alt": "https://movie.douban.com/review/9568492/",
	            "id": "9568492"
	        }
	    ],
	    "ratings_count": 182713,
	    "aka": [
	        "大富翁",
	        "诳想曲",
	        "The Island"
	    ]
	}
```

### 影片剧照

url：`https://api.douban.com/v2/movie/subject/{id}/photos`

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空
- `count`：返回的总数量（注：此时的count = start + num；num为每次返回的条数也可认为是分页时每页显示的条数）
- `start`：从第多少个开始

url 示例：[`https://api.douban.com/v2/movie/subject/26865690/photos?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=something&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/subject/26865690/photos?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=something&udid=dddddddddddddddddddddd) 或 [`https://api.douban.com/v2/movie/subject/26865690/photos?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/subject/26865690/photos?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：

```js
	{
	    "count": 5,
	    "photos": [
	        {
	            "photos_count": 12,
	            "thumb": "https://img3.doubanio.com/view/photo/m/public/p2406383762.webp",
	            "icon": "https://img3.doubanio.com/view/photo/s/public/p2406383762.webp",
	            "author": {
	                "uid": "122971558",
	                "avatar": "https://img3.doubanio.com/icon/u122971558-2.jpg",
	                "signature": "",
	                "alt": "https://www.douban.com/people/122971558/",
	                "id": "122971558",
	                "name": "FUA"
	            },
	            "created_at": "2016-12-18 20:14:19",
	            "album_id": "1638319514",
	            "cover": "https://img3.doubanio.com/view/photo/sqs/public/p2406383762.webp",
	            "id": "2406383762",
	            "prev_photo": "2408074715",
	            "album_url": "https://movie.douban.com/subject/26865690/photos",
	            "comments_count": 3,
	            "image": "https://img3.doubanio.com/view/photo/l/public/p2406383762.webp",
	            "recs_count": 1,
	            "position": 6,
	            "alt": "https://movie.douban.com/photos/photo/2406383762/",
	            "album_title": "恐怖理发店(26865690)",
	            "next_photo": "2406383761",
	            "subject_id": "26865690",
	            "desc": ""
	        }
	    ],
	    "total": 17,
	    "start": 0,
	    "subject": {
	        "rating": {
	            "max": 10,
	            "average": 2.4,
	            "details": {
	                "1": 70,
	                "2": 6,
	                "3": 3,
	                "4": 0,
	                "5": 1
	            },
	            "stars": "15",
	            "min": 0
	        },
	        "genres": [
	            "爱情",
	            "悬疑",
	            "惊悚"
	        ],
	        "title": "恐怖理发店",
	        "casts": [
	            {
	                "avatars": {
	                    "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp",
	                    "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp",
	                    "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp"
	                },
	                "name_en": "Guoer Yin",
	                "name": "殷果儿",
	                "alt": "https://movie.douban.com/celebrity/1340984/",
	                "id": "1340984"
	            }
	        ],
	        "durations": [
	            "89分钟"
	        ],
	        "collect_count": 703,
	        "mainland_pubdate": "2017-01-06",
	        "has_video": true,
	        "original_title": "恐怖理发店",
	        "subtype": "movie",
	        "directors": [
	            {
	                "avatars": {
	                    "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp",
	                    "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp",
	                    "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp"
	                },
	                "name_en": "Shilei Lu",
	                "name": "陆诗雷",
	                "alt": "https://movie.douban.com/celebrity/1360707/",
	                "id": "1360707"
	            }
	        ],
	        "pubdates": [
	            "2017-01-06(中国大陆)"
	        ],
	        "year": "2017",
	        "images": {
	            "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp",
	            "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp",
	            "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp"
	        },
	        "alt": "https://movie.douban.com/subject/26865690/",
	        "id": "26865690"
	    }
	}
```
### 电影影评列表

url：`https://api.douban.com/v2/movie/subject/{id}/reviews`

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空
- `count`：返回数量
- `start`：从第多少个开始

url 示例：
[`https://api.douban.com/v2/movie/subject/26865690/reviews?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=something&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/subject/26865690/reviews?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=something&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/subject/26865690/reviews?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/subject/26865690/reviews?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：

```js
	{
	    "count": 5,
	    "reviews": [
	        {
	            "rating": {
	                "max": 5,
	                "value": 1,
	                "min": 0
	            },
	            "useful_count": 38,
	            "author": {
	                "uid": "123404248",
	                "avatar": "https://img3.doubanio.com/icon/u123404248-5.jpg",
	                "signature": "",
	                "alt": "https://www.douban.com/people/123404248/",
	                "id": "123404248",
	                "name": "世界奇妙物语"
	            },
	            "created_at": "2017-01-19 21:46:33",
	            "title": "国产恐怖片，注定成烂片？",
	            "updated_at": "2017-04-12 15:52:33",
	            "share_url": "https://m.douban.com/movie/review/8301338",
	            "summary": "这一系列国产恐怖片太多，现在总结下国产电影拍摄门槛为什么这么低…… 1.找个导演，内地导演优先考虑(省钱)。 2.去网上热搜榜（也是经纪公司）上挑几个网红明星（省钱）。网红明星就像木偶一样被装扮上了。 3.去...",
	            "content": "这一系列国产恐怖片太多，现在总结下国产电影拍摄门槛为什么这么低……\r\n1.找个导演，内地导演优先考虑(省钱)。\r\n2.去网上热搜榜（也是经纪公司）上挑几个网红明星（省钱）。",
	            "useless_count": 1,
	            "comments_count": 2,
	            "alt": "https://movie.douban.com/review/8301338/",
	            "id": "8301338",
	            "subject_id": "26865690"
	        }
	    ],
	    "start": 0,
	    "total": 12,
	    "next_start": 5,
	    "subject": {
	        "rating": {
	            "max": 10,
	            "average": 2.4,
	            "details": {
	                "1": 70,
	                "2": 6,
	                "3": 3,
	                "4": 0,
	                "5": 1
	            },
	            "stars": "15",
	            "min": 0
	        },
	        "genres": [
	            "爱情",
	            "悬疑",
	            "惊悚"
	        ],
	        "title": "恐怖理发店",
	        "casts": [
	            {
	                "avatars": {
	                    "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp",
	                    "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp",
	                    "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp"
	                },
	                "name_en": "Guoer Yin",
	                "name": "殷果儿",
	                "alt": "https://movie.douban.com/celebrity/1340984/",
	                "id": "1340984"
	            }
	        ],
	        "durations": [
	            "89分钟"
	        ],
	        "collect_count": 703,
	        "mainland_pubdate": "2017-01-06",
	        "has_video": true,
	        "original_title": "恐怖理发店",
	        "subtype": "movie",
	        "directors": [
	            {
	                "avatars": {
	                    "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp",
	                    "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp",
	                    "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp"
	                },
	                "name_en": "Shilei Lu",
	                "name": "陆诗雷",
	                "alt": "https://movie.douban.com/celebrity/1360707/",
	                "id": "1360707"
	            }
	        ],
	        "pubdates": [
	            "2017-01-06(中国大陆)"
	        ],
	        "year": "2017",
	        "images": {
	            "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp",
	            "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp",
	            "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp"
	        },
	        "alt": "https://movie.douban.com/subject/26865690/",
	        "id": "26865690"
	    }
	}
```
### 电影短评列表

url：`https://api.douban.com/v2/movie/subject/{id}/comments`

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空
- `count`：返回数量
- `start`：从第多少个开始

url 示例：
[`https://api.douban.com/v2/movie/subject/26865690/comments?apikey=0b2bdeda43b5688921839c8ecb20399b&count=20&start=0&client=something&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/subject/26865690/comments?apikey=0b2bdeda43b5688921839c8ecb20399b&count=20&start=0&client=something&udid=dddddddddddddddddddddd) 
或
 [`https://api.douban.com/v2/movie/subject/26865690/comments?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/subject/26865690/comments?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：

```js
	{
	    "count": 5,
	    "comments": [
	        {
	            "rating": {
	                "max": 5,
	                "value": 1,
	                "min": 0
	            },
	            "useful_count": 272,
	            "author": {
	                "uid": "62598926",
	                "avatar": "https://img3.doubanio.com/icon/u62598926-1.jpg",
	                "signature": "",
	                "alt": "https://www.douban.com/people/62598926/",
	                "id": "62598926",
	                "name": "小曦讨厌下雨天"
	            },
	            "subject_id": "26865690",
	            "content": "太恐怖了！吓得我从第十分钟开始就没敢睁眼睛，最后直接睡着了。",
	            "created_at": "2017-01-06 15:16:12",
	            "id": "1132938490"
	        },
	        {
	            "rating": {
	                "max": 5,
	                "value": 1,
	                "min": 0
	            },
	            "useful_count": 143,
	            "author": {
	                "uid": "147408877",
	                "avatar": "https://img3.doubanio.com/icon/u147408877-1.jpg",
	                "signature": "",
	                "alt": "https://www.douban.com/people/147408877/",
	                "id": "147408877",
	                "name": "turnin'"
	            },
	            "subject_id": "26865690",
	            "content": "刘哔又有素材了，我先帮你占个座",
	            "created_at": "2017-01-06 14:01:18",
	            "id": "1132901642"
	        }
	    ],
	    "start": 0,
	    "total": 322,
	    "next_start": 5,
	    "subject": {
	        "rating": {
	            "max": 10,
	            "average": 2.4,
	            "details": {
	                "1": 70,
	                "2": 6,
	                "3": 3,
	                "4": 0,
	                "5": 1
	            },
	            "stars": "15",
	            "min": 0
	        },
	        "genres": [
	            "爱情",
	            "悬疑",
	            "惊悚"
	        ],
	        "title": "恐怖理发店",
	        "casts": [
	            {
	                "avatars": {
	                    "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp",
	                    "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp",
	                    "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1403756298.69.webp"
	                },
	                "name_en": "Guoer Yin",
	                "name": "殷果儿",
	                "alt": "https://movie.douban.com/celebrity/1340984/",
	                "id": "1340984"
	            }
	        ],
	        "durations": [
	            "89分钟"
	        ],
	        "collect_count": 703,
	        "mainland_pubdate": "2017-01-06",
	        "has_video": true,
	        "original_title": "恐怖理发店",
	        "subtype": "movie",
	        "directors": [
	            {
	                "avatars": {
	                    "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp",
	                    "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp",
	                    "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1490348628.29.webp"
	                },
	                "name_en": "Shilei Lu",
	                "name": "陆诗雷",
	                "alt": "https://movie.douban.com/celebrity/1360707/",
	                "id": "1360707"
	            }
	        ],
	        "pubdates": [
	            "2017-01-06(中国大陆)"
	        ],
	        "year": "2017",
	        "images": {
	            "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp",
	            "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp",
	            "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2406903891.webp"
	        },
	        "alt": "https://movie.douban.com/subject/26865690/",
	        "id": "26865690"
	    }
	}
```


### 影人信息

url：`https://api.douban.com/v2/movie/celebrity/{id}`

拼接参数：

- `apikey`：apikey
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/celebrity/1054395?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/celebrity/1054395?apikey=0b2bdeda43b5688921839c8ecb20399b&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/celebrity/1054395?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/celebrity/1054395?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：

```js

	{
	    "website": "",
	    "mobile_url": "https://movie.douban.com/celebrity/1054395/mobile",
	    "aka_en": [
	        "Elijah Jordan Wood (本名)",
	        "Elwood, Lij and Monkey (昵称)"
	    ],
	    "name": "伊莱贾·伍德",
	    "works": [
	        {
	            "roles": [
	                "演员"
	            ],
	            "subject": {
	                "rating": {
	                    "max": 10,
	                    "average": 9.3,
	                    "details": {
	                        "1": 7,
	                        "2": 5,
	                        "3": 77,
	                        "4": 360,
	                        "5": 1071
	                    },
	                    "stars": "50",
	                    "min": 0
	                },
	                "genres": [
	                    "喜剧",
	                    "短片",
	                    "音乐"
	                ],
	                "title": "SMAPxSMAP",
	                "casts": [
	                    {
	                        "avatars": {
	                            "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1941.webp",
	                            "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1941.webp",
	                            "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1941.webp"
	                        },
	                        "name_en": "Masahiro Nakai",
	                        "name": "中居正广",
	                        "alt": "https://movie.douban.com/celebrity/1023890/",
	                        "id": "1023890"
	                    }
	                ],
	                "durations": [
	                    "52分钟"
	                ],
	                "collect_count": 2601,
	                "mainland_pubdate": "",
	                "has_video": false,
	                "original_title": "SMAPxSMAP",
	                "subtype": "tv",
	                "directors": [],
	                "pubdates": [
	                    "1996-04-15"
	                ],
	                "year": "1996",
	                "images": {
	                    "small": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2375579599.webp",
	                    "large": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2375579599.webp",
	                    "medium": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2375579599.webp"
	                },
	                "alt": "https://movie.douban.com/subject/1763308/",
	                "id": "1763308"
	            }
	        },
	        {
	            "roles": [
	                "演员"
	            ],
	            "subject": {
	                "rating": {
	                    "max": 10,
	                    "average": 9.2,
	                    "details": {
	                        "1": 3,
	                        "2": 5,
	                        "3": 97,
	                        "4": 289,
	                        "5": 904
	                    },
	                    "stars": "50",
	                    "min": 0
	                },
	                "genres": [
	                    "喜剧",
	                    "爱情"
	                ],
	                "title": "欢乐一家亲 第一季",
	                "casts": [
	                    {
	                        "avatars": {
	                            "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1396501988.66.webp",
	                            "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1396501988.66.webp",
	                            "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1396501988.66.webp"
	                        },
	                        "name_en": "Kelsey Grammer",
	                        "name": "凯尔希·格兰莫",
	                        "alt": "https://movie.douban.com/celebrity/1031847/",
	                        "id": "1031847"
	                    }
	                ],
	                "durations": [
	                    "22分钟"
	                ],
	                "collect_count": 1880,
	                "mainland_pubdate": "",
	                "has_video": false,
	                "original_title": "Frasier",
	                "subtype": "tv",
	                "directors": [
	                    {
	                        "avatars": {
	                            "small": "https://img1.doubanio.com/f/movie/ca527386eb8c4e325611e22dfcb04cc116d6b423/pics/movie/celebrity-default-small.png",
	                            "large": "https://img3.doubanio.com/f/movie/63acc16ca6309ef191f0378faf793d1096a3e606/pics/movie/celebrity-default-large.png",
	                            "medium": "https://img1.doubanio.com/f/movie/8dd0c794499fe925ae2ae89ee30cd225750457b4/pics/movie/celebrity-default-medium.png"
	                        },
	                        "name_en": "David Angell",
	                        "name": "David Angell",
	                        "alt": "https://movie.douban.com/celebrity/1000586/",
	                        "id": "1000586"
	                    }
	                ],
	                "pubdates": [
	                    "1993-09-16(美国)"
	                ],
	                "year": "1993",
	                "images": {
	                    "small": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2212098341.webp",
	                    "large": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2212098341.webp",
	                    "medium": "https://img3.doubanio.com/view/photo/s_ratio_poster/public/p2212098341.webp"
	                },
	                "alt": "https://movie.douban.com/subject/1438242/",
	                "id": "1438242"
	            }
	        }
	    ],
	    "name_en": "Elijah Wood",
	    "gender": "男",
	    "professions": [
	        "演员",
	        "制片人",
	        "配音",
	        "副导演"
	    ],
	    "avatars": {
	        "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp",
	        "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp",
	        "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp"
	    },
	    "summary": "伊利亚·乔丹·伍德(Elijah Jordan Wood)，1981年1月28日出生于美国爱荷华州的锡达拉皮兹，父亲沃伦  伊利亚·伍德·伍德，母亲黛比·伍德。他在家中排行老二，上边有一个哥哥扎克，下面有一个妹妹汉纳·伍德。年幼时候，表现欲极强的伊利亚就表现出取悦别人的才能，母亲决定带他到洛杉矶，参加一年一度的国际模特人材协会大会，寻找发展机会。很快，他在好莱坞令人眼花缭乱的表演世界找到了一份工作。不久，他开始涉足商业表演，在电视表演界得到一些小的角色。",
	    "photos": [
	        {
	            "thumb": "https://img1.doubanio.com/view/photo/m/public/p2203408008.webp",
	            "image": "https://img1.doubanio.com/view/photo/l/public/p2203408008.webp",
	            "cover": "https://img1.doubanio.com/view/photo/sqs/public/p2203408008.webp",
	            "alt": "https://movie.douban.com/celebrity/1054395/photo/2203408008/",
	            "id": "2203408008",
	            "icon": "https://img1.doubanio.com/view/photo/s/public/p2203408008.webp"
	        }
	    ],
	    "birthday": "1981-01-28",
	    "aka": [
	        "伊莱贾·伍德"
	    ],
	    "alt": "https://movie.douban.com/celebrity/1054395/",
	    "born_place": "美国,爱荷华州,锡达拉皮兹",
	    "constellation": "水瓶座",
	    "id": "1054395"
	}
```


### 影人剧照

url：`https://api.douban.com/v2/movie/celebrity/{id}/photos`

拼接参数：

- `apikey`：apikey
- `count`：返回的总数量（注：此时的count = start + num；num为每次返回的条数也可认为是分页时每页显示的条数）
- `start`：从第多少个开始
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/celebrity/1054395/photos?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/celebrity/1054395/photos?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/celebrity/1054395/photos?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/celebrity/1054395/photos?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：
```js

	{
	    "count": 20,
	    "photos": [
	        {
	            "photos_count": 244,
	            "thumb": "https://img1.doubanio.com/view/photo/m/public/p2203408008.webp",
	            "icon": "https://img1.doubanio.com/view/photo/s/public/p2203408008.webp",
	            "author": {
	                "uid": "84958815",
	                "avatar": "https://img3.doubanio.com/icon/u84958815-2.jpg",
	                "signature": "",
	                "alt": "https://www.douban.com/people/84958815/",
	                "id": "84958815",
	                "name": "礼帽"
	            },
	            "created_at": "2014-10-02 20:52:11",
	            "album_id": "40868593",
	            "cover": "https://img1.doubanio.com/view/photo/sqs/public/p2203408008.webp",
	            "id": "2203408008",
	            "prev_photo": "2206619587",
	            "album_url": "https://movie.douban.com/celebrity/1054395/photos/",
	            "comments_count": 22,
	            "image": "https://img1.doubanio.com/view/photo/l/public/p2203408008.webp",
	            "recs_count": 2,
	            "position": 42,
	            "alt": "https://movie.douban.com/celebrity/1054395/photo/2203408008/",
	            "album_title": "影人图片:伊利亚·伍德 Elijah Wood",
	            "next_photo": "2188620568",
	            "subject_id": "1054395",
	            "desc": "Elijah Wood and Leonardo DiCaprio at the 1994 Academy Awards."
	        },
	        {
	            "photos_count": 244,
	            "thumb": "https://img3.doubanio.com/view/photo/m/public/p1573366851.webp",
	            "icon": "https://img3.doubanio.com/view/photo/s/public/p1573366851.webp",
	            "author": {
	                "uid": "Bill0425",
	                "avatar": "https://img3.doubanio.com/icon/u3945601-892.jpg",
	                "signature": "",
	                "alt": "https://www.douban.com/people/Bill0425/",
	                "id": "3945601",
	                "name": "Bill"
	            },
	            "created_at": "2012-06-02 20:34:36",
	            "album_id": "40868593",
	            "cover": "https://img3.doubanio.com/view/photo/sqs/public/p1573366851.webp",
	            "id": "1573366851",
	            "prev_photo": "1607526483",
	            "album_url": "https://movie.douban.com/celebrity/1054395/photos/",
	            "comments_count": 37,
	            "image": "https://img3.doubanio.com/view/photo/l/public/p1573366851.webp",
	            "recs_count": 10,
	            "position": 126,
	            "alt": "https://movie.douban.com/celebrity/1054395/photo/1573366851/",
	            "album_title": "影人图片:伊利亚·伍德 Elijah Wood",
	            "next_photo": "1489499030",
	            "subject_id": "1054395",
	            "desc": ""
	        }
	    ],
	    "celebrity": {
	        "avatars": {
	            "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp",
	            "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp",
	            "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp"
	        },
	        "name_en": "Elijah Wood",
	        "name": "伊莱贾·伍德",
	        "alt": "https://movie.douban.com/celebrity/1054395/",
	        "id": "1054395"
	    },
	    "total": 244,
	    "start": 0
	}
```

### 影人作品

url：`https://api.douban.com/v2/movie/celebrity/{id}/works`

拼接参数：

- `apikey`：apikey
- `count`：返回数量
- `start`：从第多少个开始
- `client`：客户端信息。可为空
- `udid`：用户 id。可为空

url 示例：
[`https://api.douban.com/v2/movie/celebrity/1054395/works?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd`](https://api.douban.com/v2/movie/celebrity/1054395/works?apikey=0b2bdeda43b5688921839c8ecb20399b&start=0&count=20&client=somemessage&udid=dddddddddddddddddddddd) 
或 
[`https://api.douban.com/v2/movie/celebrity/1054395/works?apikey=0b2bdeda43b5688921839c8ecb20399b`](https://api.douban.com/v2/movie/celebrity/1054395/works?apikey=0b2bdeda43b5688921839c8ecb20399b)

json 示例：

```js
	{
	    "count": 2,
	    "start": 0,
	    "celebrity": {
	        "avatars": {
	            "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp",
	            "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp",
	            "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p51597.webp"
	        },
	        "name_en": "Elijah Wood",
	        "name": "伊莱贾·伍德",
	        "alt": "https://movie.douban.com/celebrity/1054395/",
	        "id": "1054395"
	    },
	    "total": 88,
	    "works": [
	        {
	            "roles": [
	                "制片人"
	            ],
	            "subject": {
	                "rating": {
	                    "max": 10,
	                    "average": 7.2,
	                    "details": {
	                        "1": 2,
	                        "2": 3,
	                        "3": 12,
	                        "4": 7,
	                        "5": 10
	                    },
	                    "stars": "35",
	                    "min": 0
	                },
	                "genres": [
	                    "动作",
	                    "惊悚"
	                ],
	                "title": "曼蒂",
	                "casts": [
	                    {
	                        "avatars": {
	                            "small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1393937546.11.webp",
	                            "large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1393937546.11.webp",
	                            "medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1393937546.11.webp"
	                        },
	                        "name_en": "Nicolas Cage",
	                        "name": "尼古拉斯·凯奇",
	                        "alt": "https://movie.douban.com/celebrity/1054455/",
	                        "id": "1054455"
	                    }
	                ],
	                "durations": [
	                    "120分钟"
	                ],
	                "collect_count": 283,
	                "mainland_pubdate": "",
	                "has_video": false,
	                "original_title": "Mandy",
	                "subtype": "movie",
	                "directors": [
	                    {
	                        "avatars": {
	                            "small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/pdWOTUV4N7sEcel_avatar_uploaded1500967301.38.webp",
	                            "large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/pdWOTUV4N7sEcel_avatar_uploaded1500967301.38.webp",
	                            "medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/pdWOTUV4N7sEcel_avatar_uploaded1500967301.38.webp"
	                        },
	                        "name_en": "Panos Cosmatos",
	                        "name": "帕诺斯·科斯马图斯",
	                        "alt": "https://movie.douban.com/celebrity/1378255/",
	                        "id": "1378255"
	                    }
	                ],
	                "pubdates": [
	                    "2018-01-19(圣丹斯电影节)",
	                    "2018-09-14(美国)"
	                ],
	                "year": "2018",
	                "images": {
	                    "small": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2511683437.webp",
	                    "large": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2511683437.webp",
	                    "medium": "https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2511683437.webp"
	                },
	                "alt": "https://movie.douban.com/subject/27066203/",
	                "id": "27066203"
	            }
	        }
	    ]
	}
```


## 附录

### 影片信息属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
|id|	电影id|	str	|Y|	Y	|Y|	-|
|title	|中文名|	str|	Y|	Y|	Y	|-|
|original_title	|原名	|str|	Y	|Y	|Y	|''|
|aka	|又名	|array|	Y	|Y	|Y	|[]|
|alt	|条目页URL	|str	|Y	|Y	|Y	|-|
|mobile_url	|移动版条目页URL|	str	|Y|	Y|	Y|	-|
|rating	|评分，[见附录](#rating)	|dict	|Y	|Y|	Y	|-|
|ratings_count	|评分人数	|int|	Y|	Y	|Y	|0|
|wish_count	|想看人数	|int|	Y	|Y	|Y	|0|
|collect_count	|看过人数	|int|	Y	|Y	|Y	|0|
|do_count	|在看人数，如果是电视剧，默认值为0，如果是电影值为null	|int|	Y|	Y	|Y	|0 / null|
|images	|电影海报图，分别提供288px x 465px(大)，96px x 155px(中) 64px x 103px(小)尺寸	|dict|	Y	|Y|	Y|	-|
|subtype	|条目分类, movie或者tv	|str	|Y|	Y	|Y|	movie|
|directors|	导演，数据结构为影人的简化描述，[见附录](#sample_celebrity)|	array|	Y|	Y	|Y	|[]
|casts	|主演，最多可获得4个，数据结构为影人的简化描述，[见附录](#sample_celebrity)|	array	|Y	|Y	|Y|	[]
|writers|	编剧，数据结构为影人的简化描述，[见附录](#sample_celebrity)|	array	|N|	Y	|Y|	[]|
|website	|官方网站	|str|	N|	Y	|Y|	''|
|douban_site	|豆瓣小站|	str	|Y	|Y|	Y	|''|
|pubdates	|如果条目类型是电影则为上映日期，如果是电视剧则为首Ï日期|	array	|N|	Y	|Y|	[]|
|mainland_pubdate	|大陆上映日期，如果条目类型是电影则为上映日期，如果是电视剧则为首播日期|	str|	N|	Y	|Y	|''|
|pubdate|	兼容性数据，未来会去掉，大陆上映日期，如果条目类型是电影则为上映日期，如果是电视剧则为首播日期	|str|	N|	Y|	Y	|''|
|year	|年代	|str|	Y	|Y	|Y|	''|
|languages|	语言	|array|	N|	Y	|Y|	[]|
|durations	|片长|	array	|N	|Y|	Y	|[]|
|genres|	影片类型，最多提供3个|	array	|Y|	Y|	Y|	[]|
|countries|	制片国家/地区|	array	|Y|	Y|	Y|	[]|
|summary	|简介|	str	|Y	|Y	|Y|	''|
|comments_count|	短评数量	|int|	Y|	Y|	Y|	0|
|reviews_count|	影评数量	|int	|Y	|Y	|Y|	0|
|seasons_count|	总季数(tv only)	|int|	Y|	Y|	Y|	0 / null|
|current_season|	当前季数(tv only)	|int|	Y|	Y|	Y	|0 / null|
|episodes_count	|当前季的集数(tv only)	|int|	Y|	Y|	Y	|0 / null|
|schedule_url	|影讯页URL(movie only)|	str|	Y|	Y|	Y	|''|
|trailer_urls|	预告片URL，对高级用户以上开放，最多开放4个地址|	array|	N	|Y	|Y	|[]|
|clip_urls|	片段URL，对高级用户以上开放，最多开放4个地址|	array|	N|	Y|	Y	|[]
|blooper_urls	|花絮URL，对高级用户以上开放，最多开放4个地址|	array|	N|	Y	|Y|	[]|
|photos|	电影剧照，前10张，[见附录](#movie_photos)	|array|	N|	Y	|Y	|[]|
|popular_reviews	|影评，前10条，影评结构，[见附录](#popular_reviews)|	array	|N|	Y|	Y|	[]|

### 剧照属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
|id	|图片id	|str|	N/A	|Y|	Y	|-|
|subject_id	|条目id	|str|	N/A	|Y|	Y	|-|
|alt|	图片展示页url	|str|	N/A	|Y|	Y	|-|
|icon	|图片地址，icon尺寸|str|N/A|	Y	|Y	|-|
|image	|图片地址，image尺寸|str|	N/A	|Y	|Y|	-|
|thumb	|图片地址，thumb尺寸|str|N/A|Y|	Y|	-|
|cover|	图片地址，cover尺寸|str|N/A|Y|Y|	-|
|created_at	|发布日期	|str|	N/A	|Y	|Y	|-|
|desc	|图片描述|	str|	N/A|	Y	|Y	|''|
|author|上传用户，见附录|	dict|N/A	|Y	|Y|	-|
|album_id	|相册id|	str|	N/A|	Y	|Y	|-|
|album_title|	相册标题	|str	|N/A|Y	|Y	|-|
|album_url	|相册地址	|str|	N/A	|Y	|Y|	-|
|next_photo|	下一张图片	|str|	N/A	|Y|	Y	|''|
|prev_photo|	上一张图片	|str|	N/A	|Y|	Y	|''|
|position|图片在相册中的位置，按照时间排序|int|N/A|Y|Y|0|
|comments_count	|评论数	|int|N/A|Y|	Y	|0|
|photos_count|全部剧照数量|int|N/A	|Y|Y|0|


### 电影总平均评分属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
min|	最低评分|	int	|Y|	Y|	Y|-|
max	|最高评分	|int	|Y|	Y|	Y|-|
average	|评分	|float(1)		|Y|	Y|	Y|-|
stars|	评星数	|int	|Y|	Y|	Y|-|


### 电影影评属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
id	|影评id	|str|	Y	|Y	|Y|	-
title	|影评名	|str|	Y|	Y	|Y|	-
alt	|影评url	|str|	Y|	Y|	Y|	-
created_at|	发布日期	|str|	Y|	Y|	Y|	-
updated_at	|更新日期	|str|	Y	|Y|	Y|	-
subject_id	|条目id|	str|	Y|	Y	|Y|	-
author|	上传用户，[见附录](#user)	|dict	|Y	|Y|	Y	|-
summary	|摘要，100字以内|	str	|Y	|Y|	Y	|-
rating|	影评评分，[见附录](#user_rating)	|dict|	Y	|Y	|Y|	-
useful_count|	有用数	|int|	Y|	Y|	Y|	0
useless_count	|无用数	|int|	Y|	Y|	Y	|0
comments_count|	评论数	|int|	Y	|Y|	Y	|0


### 电影短评属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
id	|短评id|	str|	Y|	Y	|Y	|-
created_at|	发布日期	|str|	Y|	Y|	Y|	-
subject_id	|条目id|	str|	Y|	Y	|Y|	-
author|	上传用户，[见附录](#user)	|dict	|Y	|Y|	Y	|-
summary	|摘要，100字以内|	str	|Y	|Y|	Y	|-
rating|	影评评分，[见附录](#user_rating)	|dict|	Y	|Y	|Y|	-
useful_count|	有用数	|int|	Y|	Y|	Y|	0

### 某用户评分属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
min|	最低评分|	int	|Y|	Y|	Y|-|
max	|最高评分	|int	|Y|	Y|	Y|-|
value	|评分	|int|	Y	|Y|	Y|	-|

### 影人的简化描述属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
id	|影人条目id|	str	|Y	|Y|	Y|	-
name	|中文名|	str	|Y|	Y|	Y	|-
alt	|影人条目URL	|str	|Y|	Y	|Y	|-
avatars|	影人头像，分别提供420px x 600px(大)，140px x 200px(中) 70px x 100px(小)尺寸	|dict	|Y	|Y|	Y|	-


### 评论用户属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
id|	用户id|	str|	Y	|Y	|Y	|-
name	|用户名	|str	|Y	|Y|	Y|	-
uid|	用户唯一标识|	str|	Y	|Y|	Y|	-
signature	|用户签名	|str|	Y|	Y	|Y	|''
alt|	用户个人主页url|	str|	Y	|Y|	Y	|-
avatar	|用户头像	|str	|Y	|Y|	Y	|-

### 北美票房排行属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
rank	|排名	|int	|Y	|Y|	Y	|-
box	|票房|	int	|Y|	Y	|Y	|-
new	|是否新上映	|bool|	Y|	Y|	Y	|-
subject	|电影条目，[见附录](#subject_attr)	|dict	|Y|	Y|	Y|	-


### 口碑榜weekly条目属性字段解析

|字段|	描述|	数据类型	|公开|	高级|	商务|默认值|
|-----|-----|:-----:|:-----:|:-----:|:-----:|:-----:|
rank	|排名	|int|	Y|	Y	|Y|	-
delta	|排名改变量	|int|	Y	|Y|	Y|	-
