# 抓包分析

不论用那种方式去写爬虫代码，都要先知道：

具体需要爬取哪些url（或api等），url地址是多少

以及需要传递什么参数，才能返回我们希望的数据

而要搞清楚，要抓取哪些数据，这些数据怎么获取到，即：

* 需要访问的网页url地址是什么
  * 以及需要传递什么参数
* 对于返回数据，需要抓取具体哪一部分
  * 对应的数据的提取规则是什么

这一抓取网络请求的数据包的过程，叫做：`抓包`

## 抓包常用辅助工具

我们要写爬虫去爬取的数据，从数据源的形态分，大概分两类：

* `网站`=网页=网站中的各种网页
* `app`=app中内部发出的请求设计的api接口

根据要抓取的数据的源不同，常用的一些辅助分析工具有：

* 网站抓包分析
  * `Chrome`的`开发者工具`
    * ![Chrome的开发者工具](../assets/img/mac_chrome_dev_tools.png)
    * 快捷键：
      * Windows: `Ctrl + Shift + I`
      * Mac: `Command + Option + I`
    * 如何使用
      * 官网资料：[Chrome 开发者工具](https://developers.google.com/web/tools/chrome-devtools/?hl=zh-cn)
  * `IE`的`F12`
    * 如何使用
      * [【整理】各种浏览器中的开发人员工具Developer Tools：IE9的F12，Chrome的Ctrl+Shift+J，Firefox的Firebug](http://www.crifan.com/summary_webbrowser_developer_tool_ie9_f12_chrome_ctrl_shift_j_firefox_firebug)
      * [【总结】浏览器中的开发人员工具（IE9的F12和Chrome的Ctrl+Shift+I）-网页分析的利器](http://www.crifan.com/browser_developer_tool_chrome_vs_ie9)
      * [【教程】如何利用IE9的F12去分析网站登陆过程中的复杂的（参数，cookie等）值（的来源）](http://www.crifan.com/use_ie9_f12_to_analysis_the_root_source_of_values_of_parameter_cookie)
      * [【教程】手把手教你如何利用工具(IE9的F12)去分析模拟登陆网站(百度首页)的内部逻辑过程](http://www.crifan.com/use_ie9_f12_to_analysis_the_internal_logical_process_of_login_baidu_main_page_website)
    * `Firefox`的`firebug`
* app抓包分析
  * `Charles`
    * [app抓包利器：Charles](http://book.crifan.com/books/app_capture_package_tool_charles/website)

## 具体怎么抓包

先要搞清楚自己想要抓取什么数据，然后再去用工具辅助分析出网页或app等数据源中，如何一步步的获取对应数据，找到期间所要依次访问哪些url或api，传递什么参数，最终获取到所要的数据。

### 以抓取汽车之家中车型车型数据为例解释如何抓包

下面就以，想要抓取汽车之家网站中的车型车系数据为例，来解释，如何用抓包工具辅助分析，依次访问哪些页面，之后如何提取，才能得到我们要的数据。

TODO：

用Chrome浏览器分析过程，并截图，添加解释。