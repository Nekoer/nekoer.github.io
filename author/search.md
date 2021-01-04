## 搜索作者

GET `https://api.acgmx.com/public/search/users?word=xxx&offset=30`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| word  | String  | 搜索词  |
| offset  |  String |  显示数量 以倍数呈现 |


### 请求参数案例
`https://api.acgmx.com/public/search/users?word=百合&offset=30`

### 返回结果
```json
{
	"user_previews":[
		{
			"user":{...},
			"illusts":[,,,]}
	],
	"next_url": "https://app-api.pixiv.net/v1/search/user?word=%E7%99%BE%E5%90%88&filter=for_ios&sort=date_desc&offset=60"
}
```
