# 课表查询API

> 获取课表

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/table/ | 信息门户登录header | GET |

<hr/>

## Headers
信息门户登录headers(注意大小写)

```
    'Bigipserverpool':'139503808.20480.0000'
    'Sid':'2014210761'
    'Jsessionid': 'B6A6DF5C48AB4AD4C4001572D2611809'
    'Authorization': "Basic Base64(sid:pwd)"
```

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

``` 
   [
     {
        "id": "1" // 课程id
        "course": "xxxx" // 课程名称
        "teacher": "xxxx" // 老师名
        "weeks": "1, 2, 3,,,,,19" // 上课周 
        "day": "星期一" // 星期一到星期日
        "start": 1  // 每天课程开始时间(ex: start=1 表示早上第一节课开始)
        "during": "2" // 课程持续时间(ex: during=2 表示课程持续2节课)
        "place": "9-21" // 上课地点
        "remind": true/false // 课程是否设置为提醒。用户自定义课程可以设置提醒, 信息门户课程设为false。
        "color": 0 // 课程格子的颜色(随机生成), 0 或 1 或 2 或 3 
       }
    ]
```

## Status Code

```
    200 Ok
    500 获取课表出错
```

## Notes
