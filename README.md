# 最全的web爬虫基础知识

<img src="./image/spider.jpg" width="249"/>

## *[网络](https://github.com/nwaiting/spider-base/tree/master/http)*

### *1、http网络知识*

http网络作为爬虫最基本的常识，在平常开发爬虫程序中会一直使用到。最基础的从tcp建立网络链接，然后进行http的封包，发送数据，接收数据，解析报文，解析出http的字段，
根据http的方法、参数等做不同的处理，这个流程是需要学习和熟悉的，在爬虫程序中，碰到最多的就是网络的问题，网络知识不熟练，爬虫的进阶就会很难。

#### [1.1 TCP/IP 网络模型有哪几层](https://xiaolincoding.com/network/1_base/tcp_ip_model.html)

#### [1.2 Linux 系统是如何收发网络包的](https://xiaolincoding.com/network/1_base/how_os_deal_network_package.html)

#### [1.3 http报文](https://github.com/woai30231/http/tree/master/%E7%AC%AC%E4%B8%89%E7%AB%A0%20HTTP%E6%8A%A5%E6%96%87) 

#### [1.4 http重定向与负载均衡](https://github.com/woai30231/http/tree/master/%E7%AC%AC%E4%BA%8C%E5%8D%81%E7%AB%A0%20%E9%87%8D%E5%AE%9A%E5%90%91%E4%B8%8E%E8%B4%9F%E8%BD%BD%E5%9D%87%E8%A1%A1)

#### [1.5 http客户端识别与Cookie机制](https://github.com/woai30231/http/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E7%AB%A0%20%E5%AE%A2%E6%88%B7%E7%AB%AF%E8%AF%86%E5%88%AB%E4%B8%8ECookie%E6%9C%BA%E5%88%B6)

#### [1.6 httpURL与资源](https://github.com/woai30231/http/tree/master/%E7%AC%AC%E4%BA%8C%E7%AB%A0%20URL%E4%B8%8E%E8%B5%84%E6%BA%90)

#### [1.7 键入网址到网页显示，期间发生了什么](https://xiaolincoding.com/network/1_base/what_happen_url.html)

### *2、web服务器*

web服务就是与爬虫交互的对象，理解和熟悉了web服务的流程和原理，对于爬虫会有更加深入的理解

#### [2.1 web服务器应该做些什么](https://github.com/woai30231/http/tree/master/%E7%AC%AC%E4%BA%94%E7%AB%A0%20web%E6%9C%8D%E5%8A%A1%E5%99%A8)

#### [2.2 使用flask写一个最简单的web服务](http://www.bjhee.com/flask-1.html)

### *3、nginx反向代理*

Nginx是一款轻量级的Web 服务器/反向代理服务器及电子邮件（IMAP/POP3）代理服务器，其占有内存少，并发能力强，整体性能非常强大，在web前端服务器目前是企业的首选。

#### [3.1 nginx到底是什么](https://cloud.tencent.com/developer/news/241412) 

#### [3.2 为什么需要用nginx](https://worktile.com/kb/ask/17623.html)

#### [3.3 初探nginx架构](http://tengine.taobao.org/book/chapter_02.html)

#### [3.4 nginx怎么用](https://bbs.huaweicloud.com/blogs/326032)

#### [3.5 Nginx 是如何启动并处理http请求的](https://juejin.cn/post/6844903655615758350)

## *[前端html](https://github.com/nwaiting/spider-base/tree/master/html)*

HTML全称为超文本标记语言（HyperText Markup Language），是一种用于创建网页的标准标记语言。
HTML是一种基础技术，常与CSS、JavaScript一起被众多网站用于设计网页、网页应用程序以及移动应用程序的用户界面。 网页浏览器可以读取HTML文件，并将其渲染成可视化网页。
HTML描述了一个网站的结构语义随着线索的呈现，使之成为一种标记语言而非编程语言。

### [1、html基础知识](https://github.com/LiHongyao/HTML)

### [2、html解析](https://www.cnblogs.com/qlqwjy/p/16518736.html)

## *[前端js](https://github.com/nwaiting/spider-base/tree/master/js)*

js全称是JavaScript，JavaScript 是开发人员用来制作交互式网页的编程语言。从刷新社交媒体馈送到显示动画和交互式地图，JavaScript 函数可以改善网站的用户体验。作为一种客户端脚本语言，它是万维网的核心技术之一。

### [1、js基础知识](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/First_steps/What_is_JavaScript)

### [2、js分析](https://pythonjishu.com/nhhtxcqzdm/)

### [3、js加解密](https://pythonjishu.com/nhhtxcqzdm/)

### [4、js混淆和反混淆](https://segmentfault.com/a/1190000018732039)


## *[编程语言python](https://github.com/nwaiting/spider-base/tree/master/python)*

爬虫是一种技术，不一定非要跟哪个语言绑定，python作为一种广泛使用的编程语言，在爬虫领域应用也非常广泛，所以介绍了一种语言python，也有js、java的爬虫，但是学习了python，开发爬虫程序也已经足够了。

### [1、python编程实现爬虫](https://github.com/nwaiting/spider-base/tree/master/python)

### [2、ua介绍](https://github.com/nwaiting/spider-base/tree/master/python)

### [3、proxy介绍](https://github.com/nwaiting/spider-base/tree/master/python)

### [4、正则解析](https://github.com/nwaiting/spider-base/tree/master/python)


## *[工具chrome](https://github.com/nwaiting/spider-base/tree/master/chrome)*

Chrome DevTools作为一个最基本最常用的web分析工具，

### [1、定位请求](https://segmentfault.com/q/1010000009266553)

### [2、分析请求](https://github.com/morrain/chrome-devtools/blob/master/%E9%80%90%E6%AD%A5%E6%89%A7%E8%A1%8C.md)

### [3、模拟请求](https://www.v2ex.com/t/904090)

### [4、调式请求](https://github.com/morrain/chrome-devtools/blob/master/%E4%BB%A3%E7%A0%81%E8%B0%83%E8%AF%95.md)

## *[工具fiddler](https://github.com/nwaiting/spider-base/tree/master/fiddler)*

Fiddler是一款免费的互联网调试代理工具，是一款国外软件，原版软件无中文版，但有汉化版。它不仅可以抓取你电脑甚至手机与互联网的各种http通讯，同时还能查看他们进行分析。在必要的时候，你甚至可以修改（伪造）某些通讯实现前后端开发者调试的作用。其他作用比如解密https协议会话。

### [1、fiddle介绍](https://github.com/xxxily/Fiddler-plus/blob/master/doc/Fiddler%E6%95%99%E7%A8%8B.md)

### [2、抓取请求](http://testingpai.com/article/1595507292210)

### [3、分析请求](http://testingpai.com/article/1595507292210#toc_h2_8)

### [4、模拟请求](https://yoyoyoky.github.io/2017/12/09/%E7%8E%A9%E8%BD%ACFiddler-Composer%E5%8F%91%E9%80%81HTTP-Request/)


## *[数据库](https://github.com/nwaiting/spider-base/tree/master/database)*

### [1、MySQL关系型数据存储](https://github.com/jaywcjlove/mysql-tutorial)
MySQL在过去由于性能高、成本低、可靠性好，已经成为最流行的开源数据库，因此被广泛地应用在Internet上的中小型网站中，
是最流行的关系型数据库管理系统，在WEB应用方面MySQL是最好的RDBMS(Relational Database Management System：关系数据库管理系统)应用软件之一。

### [2、redis临时性数据缓存](https://github.com/WeihanLi/StackExchange.Redis-docs-zh-cn)
Redis是一个开源（BSD协议）的内存 数据结构存储，可用作数据库、缓存和消息中间件。
Redis是一个使用ANSI C编写的开源、支持网络、基于内存、可选持久性的键值对存储数据库。

### [3、mongodb文档型数据存储](https://github.com/mongodb-china/MongoDB-CN-Manual/tree/master/docs)  [文档操作](https://zdq0394.github.io/middleware/mongo/doc.html)
MongoDB 是一个基于分布式文件存储的数据库。由 C++ 语言编写。旨在为WEB应用提供可扩展的高性能数据存储解决方案。
MongoDB 是一个介于关系数据库和非关系数据库之间的产品，是非关系数据库当中功能最丰富，最像关系数据库的。它支持的数据结构非常松散，是类似Json的Bson格式，因此可以存储比较复杂的数据类型。


## 加入学习圈子,相互交流,相互学习,相互分享
<figure>
<img src="./image/wx.png" width=249/>
<img src="./image/notes.png" width=249/>
</figure>

