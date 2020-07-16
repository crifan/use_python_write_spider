# Python爬虫简介

[爬取你要的数据：爬虫技术](http://book.crifan.com/books/crawl_your_data_spider_technology/website)中已经解释了爬虫的核心步骤了和相关涉及内容，也提到了很多语言都可以实现爬虫，都能爬取到你要的数据。

不过不同语言有自己的侧重点，而其中爬虫领域，最方便的要数**Python**。Python在爬虫领域，有很多的现成的库和框架可供使用，便于快速高效的实现爬虫的功能。

## 用Python写爬虫的不同方式

正如[爬取你要的数据：爬虫技术](http://book.crifan.com/books/crawl_your_data_spider_technology/website)中所整理的，用Python去写爬虫，也有三种方式：

* **裸写**Python爬虫代码
  * 下载
    * python的内置http网络库
      * [urllib](https://docs.python.org/3/library/urllib.html)
        * [crifanLibPython](https://github.com/crifan/crifanLibPython/)中的[getUrlRespHtml](https://github.com/crifan/crifanLibPython/blob/master/crifanLib/crifanHttp.py)
  * 提取
    * [re](https://docs.python.org/3/library/re.html)模块
      * [Python中的正则表达式：re模块详解](http://book.crifan.com/books/python_regular_expression_re_intro/website)
  * 保存
    * `txt`
    * `csv` / `excel`
      * [Python心得：操作CSV和Excel](http://book.crifan.com/books/python_experience_csv_excel/website)
* 用各种**Python库**组合去写爬虫代码
  * 下载
    * 选择第三方的、更强大的、更好用的网络库
      * [Python心得：http网络库](http://book.crifan.com/books/python_experience_http_lib/website)
        * [Requests](http://docs.python-requests.org/)
        * [aiohttp](https://github.com/aio-libs/aiohttp)
  * 提取
    * [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/index.zh.html)
      * [Python专题教程：BeautifulSoup详解](https://www.crifan.com/files/doc/docbook/python_topic_beautifulsoup/release/html/python_topic_beautifulsoup.html)
        * v3 -> Python2
        * v4 -> Python3
    * [PyQuery](https://pythonhosted.org/pyquery/)
      * [Python心得：HTML解析库PyQuery](http://book.crifan.com/books/python_html_parse_pyquery/website)
    * [lxml](https://lxml.de/index.html)
      * [【记录】Python中尝试用lxml去解析html – 在路上](https://www.crifan.com/python_try_lxml_parse_html/)
    * 等等
  * 保存
    * `csv` / `excel`
    * [PyMySQL](https://github.com/PyMySQL/PyMySQL)
      * [主流关系数据库：MySQL](http://book.crifan.com/books/popular_rmdb_mysql/website/)
    * [PyMongo](https://api.mongodb.com/python/current/)
      * [主流文档型数据库：MongoDB](http://book.crifan.com/books/popular_document_db_mongodb/website)
    * 等等
* 用**爬虫框架**去写爬虫代码
  * 常见Python爬虫框架
    * [PySpider](http://docs.pyspider.org/en/latest/)
      * [Python爬虫框架：PySpider](https://book.crifan.com/books/python_spider_pyspider/website/)
    * [Scrapy](https://scrapy.org)
      * [主流Python爬虫框架：Scrapy](http://book.crifan.com/books/python_spider_scrapy/website)
    * 其他相关
      * [【整理】pyspider vs scrapy](http://www.crifan.com/python_spider_framework_pyspider_vs_scrapy)
