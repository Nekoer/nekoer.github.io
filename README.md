## 调用频率（所有接口均适用）
| 令牌  |  时间/分钟 | 调用次数  |
| :------------: | :------------: | :------------: |
| token（需申请）  | 1  | 300  |
| ip  | 1  | 100  |
| 无ip/公共调用  | 1  | 50  |

token请添加在header头部信息中，key为token。

ip无需添加到header头部信息，接口会自动获取。

[自助申请地址(需注册)](https://www.acg-gov.com/account "申请地址(需注册)")

# 公共接口

------------


## 排行榜

GET `https://api.pixiv.hcyacg.com/public/ranking`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| ranking_type  | String  | 排行榜类别  |
| mode  |  String |  模式 |
| page  |  String | 起始页面  |
| per_page  | String  | 每个页面的数据数量  |
| date  | String  | 日期 例：2020-04-13  |

#### 1. ranking_type字段
| ranking_type字段  | 排行榜类别  |
| :------------: | :------------: |
|  all | 所有  |
| illust  |  插画 |
| manga  |  漫画 |
| ugoira  | 动图  |

#### 2. mode字段
|  mode字段 | 模式  |
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

# 插画

------------

## 1.排行榜
GET ` https://api.pixiv.hcyacg.com/illust/ranking`
### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| mode  |  String |  模式 |
| date  |  String | 日期 例：2020-04-13  |
| offset  | String  | (n-1)*30  |

#### mode字段
|  mode字段 | 模式  |
| :------------: | :------------: |
| day  | 每日  |
| week  | 每周  |
| month  | 每月  |
|  week_rookie |  每周新画师 |
| week_original  | 每周原创  |
| day_male  |  每日男性向 |
| day_female  |  每日女性向 |
|  day_manga | 每日漫画  |

### 请求参数案例
`https://api.pixiv.hcyacg.com/illust/ranking?mode=day&date=2020-05-13`


## 2.查看插画高清图

GET `https://api.pixiv.hcyacg.com/illust/look`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| illustId  |  String |  插画id |
| type  |  String | 清晰度选择，默认为original|
| page  | String  | 页码(用于套图) 默认为1 |

####type字段
|  type字段 | 图片清晰度  |
| :------------: | :------------: |
| square  | 小  |
| medium  | 中  |
| large  | 大  |
|  original |  源图 |
