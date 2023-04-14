# python

## python编程实现最简单的爬虫
```python
# 采集百度热搜
import requests
headers = {
"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36"
}
url = 'https://top.baidu.com/board'
response = requests.get(url, headers=headers)
print(response.status_code)
print(response.text)
```

## [ua介绍](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Headers/User-Agent)
ua即User-Agent, User-Agent首部包含了一个特征字符串，用来让网络协议的对端来识别发起请求的用户代理软件的应用类型、操作系统、软件开发商以及版本号。

## [ua能解析出什么信息](https://www.lzltool.com/UserAgent)

## 如何通过ua禁止爬虫

禁止爬虫有动态和静态的禁止
1、静态静止：
    直接通过在nginx等代理服务器上配置ua规则直接禁止匹配规则的代理无法访问
```editorconfig
# 禁止Scrapy、baidu爬虫访问
if ($http_user_agent ~* "Scrapy|Baiduspider") {
  return 403;
}
# 禁止指定的ua爬虫和UA为空的访问
if ($http_user_agent ~ "Python-urllib|YYSpider|HttpClient|EasouSpider|^$" )
{
  return 403;
}
# 禁止非GET|HEAD|POST请求方式的抓取
if ($request_method !~ ^(GET|HEAD|POST)$) {
  return 403;
}
```
2、动态禁止
    动态禁止需要接入内部的安全系统，在处理请求前用安全系统判断此链接是否是正常访问、机器人还是程序自动访问

## [各种系统的ua列表](https://github.com/fengzhizi715/user-agent-list)

```python
# 解析百度热搜
import requests
from lxml import etree
headers = {
    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36"
}
url = 'https://top.baidu.com/board'
response = requests.get(url, headers=headers)
print(response.status_code)
html = etree.HTML(response.content)
for it in html.xpath('//div[@class="normal_1fQqB"]//div[@class="c-single-text-ellipsis"]/text()'):
    print(it)
```


## 正则解析
```python
# 解析百度热搜
import requests
from lxml import etree
headers = {
    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36"
}
url = 'https://top.baidu.com/board'
response = requests.get(url, headers=headers)
print(response.status_code)
html = etree.HTML(response.content)
for it in html.xpath('//div[@class="normal_1fQqB"]//div[@class="c-single-text-ellipsis"]/text()'):
    print(it)
```

## 代理介绍

爬虫程序在爬取数据时，经常需要对同一个站点进行多次高频率的访问，而这种访问很容易被站点服务器所识别出，然后拉黑封锁。而通过代理IP就可以让站点服务器认为每一次访问都来自于不同的用户，从而避免站点服务器的封锁。

### [免费的代理测试资源(勿压测和生产使用)](https://github.com/jhao104/proxy_pool)

```python
# 使用代理改变请求IP
import requests
proxies = {
    "http": "http://183.221.242.102:9443",
    "https": "http://183.221.242.102:9443"
}
url = 'https://myip.ipip.net'
response = requests.get(url, proxies=proxies)
print(response.text)
```
