### 请求的根路径

> http://www.liulongbin.top:3006



 

 
### 新闻列表

+ 接口URL：  /api/news
+ 调用方式： GET
+ 参数格式：无
+ 响应格式：

| 数据名称  | 数据类型 | 说明                                         |
| --------- | -------- | -------------------------------------------- |
| status    | Number   | 200 获取新闻列表成功；500 获取新闻列表失败！ |
| msg       | String   | 对 status 字段的详细说明                     |
| data      | Array    | 新闻列表数组                                 |
| +id       | Number   | 新闻Id                                       |
| +title    | String   | 新闻标题                                     |
| +source   | String   | 新闻来源                                     |
| +cmtcount | Number   | 评论数量                                     |
| +tags     | String   | 标签                                         |
| +img      | String   | 图片地址                                     |
| +time     | String   | 发表时间                                     |

+ 返回示例：

```json
{
    "status": 200,
    "msg": "获取新闻列表成功",
    "data": [
        {
            "id": 1,
            "title": "5G商用在即，三大运营商营收持续下降",
            "source": "新京报经济新闻",
            "cmtcount": 58,
            "tags": "三大运营商,中国移动,5G商用",
            "img": "/images/1.webp",
            "time": "2019-10-28T03:50:28.000Z"
        }
    ]
}
```

