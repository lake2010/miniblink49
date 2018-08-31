# 简介 Abstract

miniblink是一个开源、单文件、目前已知的最小的基于chromium的，浏览器控件。

miniblink is a open source, one file, small browser widget base on chromium.

通过导出的纯C接口，可以几行代码创建一个浏览器控件。

By using C interface, you can create a browser just some line code.

您可以通过官网https://weolar.github.io/miniblink/ 来获取关于miniblink更多的信息

more information at https://weolar.github.io/miniblink/

----

# 特性 Features

- 极致小巧的体积 small size
- C++，C#，Delphi等语言调用 C++，C#，Delphi language to call
- 内嵌Nodejs，支持electron 
- 随心所欲的定制功能、模拟环境
- 支持Windows xp、npapi
- 完善的HTML5支持，对各种前端库友好
- 关闭跨域开关后，可以使用各种跨域功能
- 整合融入nodejs，可以无缝使用nodejs各种开源框架
- 网络资源拦截，替换任意网站任意js为本地文件
- 可无缝模拟移动环境
- headless模式，极大节省资源，适用于爬虫

----

# 文档

关于miniblink的介绍见这篇文章：https://zhuanlan.zhihu.com/p/22611497?group_id=764036386641707008

API文档见：https://weolar.github.io/miniblink/doc-main.html 

----

# 使用
请前往https://github.com/weolar/miniblink49/releases 下载最新编译后的SDK，里面的demo_src是个完整的用例。

最简单的创建一个窗口：

**Usage**

```cpp
// 无边框窗体 borderless window
wkeWebView window = wkeCreateWebWindow(WKE_WINDOW_TYPE_TRANSPARENT, NULL, 0, 0, 640, 480);  
wkeLoadURLW(window, L"miniblink.net");
```
![demo-1](https://weolar.github.io/miniblink/assets/images/demo-0.gif)

# 编译

不推荐自己编译。因为每天有大量更新，我无法确保每次更新都能保证编译通过。如果有编译错误，请等待我的下次提交。

----

# mini-electron

mini-electron项目是一个基于miniblink的独立项目，旨在创建一个更小的electron运行环境。目前已经实现了这一目标。

通过替换mini-electron，打包完后的文件仅仅6m左右。

----

# 联系方式

大家有问题可以选择：

- 加Q群94093808

- 邮箱weolar@qq.com

- github里留言issue讨论

- 关注知乎专栏：https://zhuanlan.zhihu.com/chrome

----

# 致谢

特别感谢网友zero，他是miniblink的代码的重要共享者。

感谢网友core，感谢网友“大清知府”。

感谢网友boxue（ https://www.zhihu.com/people/coltor/ ），他致力于在微信小程序里推广miniblink架构。


