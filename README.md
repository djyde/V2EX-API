#V2EX Non-official API list
V2EX非官方API列表，仅供参考，欢迎补充。

#Site

###取网站信息

**/api/site/info.json**

```
{
    "title" : "V2EX",
    "slogan" : "way to explore",
    "description" : "创意工作者们的社区",
    "domain" : "www.v2ex.com"
}
```

###取网站状态

**/api/site/stats.json**

```
{
    "topic_max" : 126172,
    "member_max" : 71033
}
```

#Node

###取所有节点

**/api/nodes/all.json**

```
[

  {
      "id" : 1,
      "name" : "babel",
      "url" : "http://www.v2ex.com/go/babel",
      "title" : "Project Babel",
      "title_alternative" : "Project Babel",
      "topics" : 1102,
      "header" : "Project Babel \u002D 帮助你在云平台上搭建自己的社区",
      "footer" : "V2EX 基于 Project Babel 驱动。Project Babel 是用 Python 语言写成的，运行于 Google App Engine 云计算平台上的社区软件。Project Babel 当前开发分支 2.5。最新版本可以从 \u003Ca href\u003D\u0022http://github.com/livid/v2ex\u0022 target\u003D\u0022_blank\u0022\u003EGitHub\u003C/a\u003E 获取。",
      "created" : 1272206882
  }
]
```

###取节点信息

**/api/nodes/show.json**

| 参数（选其一）  |  |
| ------------- | ------------- |
| id | 节点id   |
| name | 节点名 |


```
{
    "id" : 2,
    "name" : "v2ex",
    "url" : "http://www.v2ex.com/go/v2ex",
    "title" : "V2EX",
    "title_alternative" : "V2EX",
    "topics" : 2000,
    
        "header" : "这里讨论和发布关于 V2EX 站点发展。",
    
    
        "footer" : null,
    
    "created" : 1272207021
}
```

#Topic

###取最新主题

**/api/topics/latest.json**

```
[
    
    {
        "id" : 128177,
        "title" : "vim\u002Dtranslator",
        "url" : "http://www.v2ex.com/t/128177",
        "content" : "一个轻巧的vim下的翻译和发音插件，依赖于 google\u002Dtranslator\u002Dcli，或者其他的命令行翻译，查询工具。发音取自google...\u000D\u000A\u000D\u000Ahttps://github.com/farseer90718/vim\u002Dtranslator\u000D\u000A\u000D\u000A功能比较简单。暂时只是实现了个人的需求...",
        "content_rendered" : "一个轻巧的vim下的翻译和发音插件，依赖于 google\u002Dtranslator\u002Dcli，或者其他的命令行翻译，查询工具。发音取自google...\u003Cbr /\u003E\u003Cbr /\u003E\u003Ca target\u003D\u0022_blank\u0022 href\u003D\u0022https://github.com/farseer90718/vim\u002Dtranslator\u0022 rel\u003D\u0022nofollow\u0022\u003Ehttps://github.com/farseer90718/vim\u002Dtranslator\u003C/a\u003E\u003Cbr /\u003E\u003Cbr /\u003E功能比较简单。暂时只是实现了个人的需求...",
        "replies" : 0,
        "member" : {
            "id" : 67060,
            "username" : "farseer2014",
            "tagline" : "",
            "avatar_mini" : "//cdn.v2ex.com/avatar/6766/2b3d/67060_mini.png?m=1408121347",
            "avatar_normal" : "//cdn.v2ex.com/avatar/6766/2b3d/67060_normal.png?m=1408121347",
            "avatar_large" : "//cdn.v2ex.com/avatar/6766/2b3d/67060_large.png?m=1408121347"
        },
        "node" : {
            "id" : 17,
            "name" : "create",
            "title" : "分享创造",
            "title_alternative" : "Create",
            "url" : "http://www.v2ex.com/go/create",
            "topics" : 2621,
            "avatar_mini" : "//cdn.v2ex.com/navatar/70ef/df2e/17_mini.png?m=1388448923",
            "avatar_normal" : "//cdn.v2ex.com/navatar/70ef/df2e/17_normal.png?m=1388448923",
            "avatar_large" : "//cdn.v2ex.com/navatar/70ef/df2e/17_large.png?m=1388448923"
        },
        "created" : 1408122614,
        "last_modified" : 1408122614,
        "last_touched" : 1408122434
    }
]
```

###取主题信息

**/api/topics/show.json**

| 参数  |  |
| ------------- | ------------- |
| id | 主题id（必选）   |

```
[{
    
    "id" : 1000,
    "title" : "Google App Engine x MobileMe",
    "url" : "http://www.v2ex.com/t/1000",
    "content" : "从现在开始，新上传到 V2EX 的头像将存储在 MobileMe iDisk 中。这是 V2EX 到目前为之所用到的第三个云。\u000D\u000A\u000D\u000A得益于这个架构升级，现在头像上传之后，将立刻在全站的所有页面更新。",
    "content_rendered" : "从现在开始，新上传到 V2EX 的头像将存储在 MobileMe iDisk 中。这是 V2EX 到目前为之所用到的第三个云。\u000D\u000A\u003Cbr /\u003E\u000D\u000A\u003Cbr /\u003E得益于这个架构升级，现在头像上传之后，将立刻在全站的所有页面更新。",
    "replies" : 14,
    "member" : {
        "id" : 1,
        "username" : "Livid",
        "tagline" : "Beautifully Advance",
        "avatar_mini" : "//cdn.v2ex.com/avatar/c4ca/4238/1_mini.png?m=1401650222",
        "avatar_normal" : "//cdn.v2ex.com/avatar/c4ca/4238/1_normal.png?m=1401650222",
        "avatar_large" : "//cdn.v2ex.com/avatar/c4ca/4238/1_large.png?m=1401650222"
    },
    "node" : {
        "id" : 1,
        "name" : "babel",
        "title" : "Project Babel",
        "url" : "http://www.v2ex.com/go/babel",
        "topics" : 1102,
        "avatar_mini" : "//cdn.v2ex.com/navatar/c4ca/4238/1_mini.png?m=1370299418",
        "avatar_normal" : "//cdn.v2ex.com/navatar/c4ca/4238/1_normal.png?m=1370299418",
        "avatar_large" : "//cdn.v2ex.com/navatar/c4ca/4238/1_large.png?m=1370299418"
    },
    "created" : 1280192329,
    "last_modified" : 1335004238,
    "last_touched" : 1280285385
    
}]
```

###根据提供信息取主题

**/api/replies/show.json**

| 参数（选其一）  |  |
| ------------- | ------------- |
| username  | 根据用户名取该用户所发表主题  |
| node_id  | 根据节点id取该节点下所有主题  |
| node_name | 根据节点名取该节点下所有主题 |


#Replies

###取主题回复

**/api/replies/show.json**

| 参数  |   |
| ------------- | ------------- |
| topic_id  | 主题id（必选）  |
| page |  |
| page_size |  |

```
[
    
    {
        "id" : 1,
        "thanks" : 5,
        "content" : "很高兴看到 v2ex 又回来了，等了你半天发第一贴了，憋死我了。\u000D\u000A\u000D\u000Anice work~",
        "content_rendered" : "很高兴看到 v2ex 又回来了，等了你半天发第一贴了，憋死我了。\u003Cbr /\u003E\u003Cbr /\u003Enice work~",
        "member" : {
            "id" : 4,
            "username" : "Jay",
            "tagline" : "",
            "avatar_mini" : "//cdn.v2ex.com/avatar/a87f/f679/4_mini.png?m=1325831331",
            "avatar_normal" : "//cdn.v2ex.com/avatar/a87f/f679/4_normal.png?m=1325831331",
            "avatar_large" : "//cdn.v2ex.com/avatar/a87f/f679/4_large.png?m=1325831331"
        },
        "created" : 1272207477,
        "last_modified" : 1335092176
    }
]
```

#Members

###取用户信息

**/api/members/show.json**

| 参数  |  |
| ------------- | ------------- |
| username  | 用户名（必选）  |

```
{
    "status" : "found",
    "id" : 16147,
    "url" : "http://www.v2ex.com/member/djyde",
    "username" : "djyde",
    "website" : "https://djyde.github.io",
    "twitter" : "",
    "location" : "",
    "tagline" : "",
    "bio" : "喜欢摄影和写作的程序员。",
    "avatar_mini" : "//cdn.v2ex.com/avatar/ed4c/1b66/16147_mini.png?m=1329639748",
    "avatar_normal" : "//cdn.v2ex.com/avatar/ed4c/1b66/16147_normal.png?m=1329639748",
    "avatar_large" : "//cdn.v2ex.com/avatar/ed4c/1b66/16147_large.png?m=1329639748",
    "created" : 1328075793
}
```
