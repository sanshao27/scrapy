# scrapy
Scrapy：Python的爬虫框架

# 实例Demo 
抓取：汽车之家、瓜子、链家 等数据信息

# 版本+环境库
Python2.7 + Scrapy1.12

初窥Scrapy
Scrapy是一个为了爬取网站数据，提取结构性数据而编写的应用框架。 可以应用在包括数据挖掘，信息处理或存储历史数据等一系列的程序中。

其最初是为了 网络抓取 所设计的， 也可以应用在获取API所返回的数据(例如 Amazon Associates Web Services ) 或者通用的网络爬虫。

# -*- coding: utf-8 -*-

# Define here the models for your scraped items
#
# See documentation in:
# http://doc.scrapy.org/en/latest/topics/items.html

import scrapy


class TrunksItem(scrapy.Item):
    # define the fields for your item here like:
    # name = scrapy.Field()
    pass


网络爬虫，是在网上进行数据抓取的程序，使用它能够抓取特定网页的HTML数据。虽然我们利用一些库开发一个爬虫程序，但是使用框架可以大大提高效率，缩短开发时间。Scrapy是一个使用Python编写的，轻量级的，简单轻巧，并且使用起来非常的方便。

Scrapy主要包括了以下组件：

引擎，用来处理整个系统的数据流处理，触发事务。
调度器，用来接受引擎发过来的请求，压入队列中，并在引擎再次请求的时候返回。
下载器，用于下载网页内容，并将网页内容返回给蜘蛛。
蜘蛛，蜘蛛是主要干活的，用它来制订特定域名或网页的解析规则。
项目管道，负责处理有蜘蛛从网页中抽取的项目，他的主要任务是清晰、验证和存储数据。当页面被蜘蛛解析后，将被发送到项目管道，并经过几个特定的次序处理数据。
下载器中间件，位于Scrapy引擎和下载器之间的钩子框架，主要是处理Scrapy引擎与下载器之间的请求及响应。
蜘蛛中间件，介于Scrapy引擎和蜘蛛之间的钩子框架，主要工作是处理蜘蛛的响应输入和请求输出。
调度中间件，介于Scrapy引擎和调度之间的中间件，从Scrapy引擎发送到调度的请求和响应。
使用Scrapy可以很方便的完成网上数据的采集工作，它为我们完成了大量的工作，而不需要自己费大力气去开发。

官方网站：http://scrapy.org/
开源地址：https://github.com/scrapy/scrapy
本代码地址:https://github.com/asen477/scrapy

# 抓取切勿干非法之事，开源仅供参考。
