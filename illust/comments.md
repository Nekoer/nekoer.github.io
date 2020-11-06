
## 评论

GET `https://api.acg-gov.com/illusts/comments`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| illustId  |  Integer |  插画id |
| offset  |  Integer |  页码30/60/90/120……默认30 |
| include_total_comments  |  boolean |  包括总评论，默认false |

### 请求参数案例
`https://api.acg-gov.com/illusts/comments?illustId=59580629&offset=30&include_total_comments=false`
