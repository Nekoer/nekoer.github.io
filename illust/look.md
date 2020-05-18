
## 查看插画高清图

GET `https://api.pixiv.hcyacg.com/illust/look`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| illustId  |  String |  插画id |
| type  |  String | 清晰度选择，默认为original|
| page  | String  | 页码(用于套图) 默认为1 |

#### type字段

|  type字段 | 图片清晰度  |
| :------------: | :------------: |
| square  | 小  |
| medium  | 中  |
| large  | 大  |
|  original |  源图 |

### 请求参数案例
`https://api.pixiv.hcyacg.com/illust/look?illustId=80723529&page=1&type=original`