# Banner获取API

> 获取banner

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/banner/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    [
        {
          "img": "http://muxistatic.com",  // 图片外链
          "url": "http://muxistudio.com",  // 图片指向链接
          "num": "1",                      // Banner出现顺序(越小越先出现)
          "update": 时间戳                 // 图片更新时间戳
        },
        {....}
    ]

## Status Code

    200 OK
    502 服务器端异常

## Notes
