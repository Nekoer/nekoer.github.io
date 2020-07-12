## 排行榜

GET `https://api.pixiv.hcyacg.com/public/ranking`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| ranking_type  | String  | 排行榜类别  |
| mode  |  String |  模式 |
| page  |  Integer | 起始页面  |
| per_page  | Integer  | 每个页面的数据数量  |
| date  | String  | 日期 例：2020-04-13  |

#### ranking_type字段
| 排行榜类别  | 描述  |
| :------------: | :------------: |
|  all | 所有  |
| illust  |  插画 |
| manga  |  漫画 |
| ugoira  | 动图  |

#### mode字段
|  模式 | 描述  |
| :------------: | :------------: |
| daily  | 每日  |
| weekly  | 每周  |
| monthly  | 每月  |
|  rookie |  新画师 |
| original  | 原创  |
| male  |  男性向 |
| female  |  女性向 |
|  daily_r18 | 每日工口  |
| weekly_r18  |  每周工口 |
| male_r18  | 男性工口  |
| female_r18 |  女性腐向 |
| r18g  | 工口加强型（猎奇）  |

### 请求参数案例
`https://api.pixiv.hcyacg.com/public/ranking?ranking_type=illust&mode=daily&date=2020-04-13&per_page=50&page=1`

### 返回结果
```json
{"status":"success","response":[{"content":"illust","mode":"daily","date":"2020-04-13","works":[{"rank":1,"previous_rank":2,"work":{"id":80723464,"title":"鬼","caption":null,"tags":["鬼滅の刃","竈門炭治郎","鬼の王","ネタバレ","鬼化炭治郎","鬼滅の刃20000users入り"],"tools":null,"image_urls":{"px_128x128":"https://i.pximg.net/c/128x128/img-master/img/2020/04/14/23/04/20/80723464_p0_square1200.jpg","px_480mw":"https://i.pximg.net/c/480x960/img-master/img/2020/04/14/23/04/20/80723464_p0_master1200.jpg","large":"https://i.pximg.net/img-original/img/2020/04/14/23/04/20/80723464_p0.jpg"},"width":716,"height":1062,"stats":{"scored_count":5293,"score":52930,"views_count":79628,"favorited_count":{"public":null,"private":null},"commented_count":null},"publicity":0,"age_limit":"all-age","created_time":"2020-04-12 00:13:00","reuploaded_time":"2020-04-14 23:04:20","user":{"id":24218478,"account":"wan_ke","name":"￦ANKE","is_following":null,"is_follower":null,"is_friend":null,"is_premium":null,"profile_image_urls":{"px_170x170":"https://i.pximg.net/user-profile/img/2019/10/22/04/04/45/16445257_404ce224320f5dac49b6715fafd3824d_170.jpg","px_50x50":"https://i.pximg.net/user-profile/img/2019/10/22/04/04/45/16445257_404ce224320f5dac49b6715fafd3824d_50.jpg"},"stats":null,"profile":null},"is_manga":null,"is_liked":null,"favorite_id":null,"page_count":2,"book_style":"none","type":"illustration","metadata":null,"content_type":null,"sanity_level":"white"}}]}],"count":1,"pagination":{"previous":null,"next":2,"current":1,"per_page":1,"total":500,"pages":500}}
```
