
## 详细数据

GET `https://api.pixiv.hcyacg.com/illusts/detail`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| illustId  |  Integer |  插画id |
|reduction | boolean| true则返回pixiv原始数据，否则默认返回本站数据|


### 请求参数案例
```http
https://api.pixiv.hcyacg.com/illusts/detail?illustId=59580629
```

```http
在头部添加
{authorization:用户token,不是APIKEY} 用于获取有趣的图
```
