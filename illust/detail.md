
## 详细数据

GET `https://api.pixiv.hcyacg.com/illust/detail`

### 请求参数
| 字段  | 类型  | 描述  |
| :------------: | :------------: | :------------: |
| illustId  |  Integer |  插画id |
|authorization | String| 用户token|


### 请求参数案例
```http
https://api.pixiv.hcyacg.com/illust/detail?illustId=59580629
```

```http
在头部添加
{authorization:token}
```
