## 排行榜
GET ` https://api.pixiv.hcyacg.com/illusts/ranking`
### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| mode  |  String |  模式 |
| date  |  Date | 日期 例：2020-04-13  |
| offset  | Integer  | (n-1)*30  |

#### mode字段
|  模式 | 描述  |
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
`https://api.pixiv.hcyacg.com/illusts/ranking?mode=day&date=2020-05-13`
