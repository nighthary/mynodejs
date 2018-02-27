# mynodejs

![awesome](https://raw.githubusercontent.com/github/explore/c304601f028774885ef27f72e6fe2d331729d8bc/topics/awesome/awesome.png)

* 免费域名解析: http://www.freenom.com/en/index.html
  498745097@qq.com yhq123456

* 汇智网: http://www.hubwiz.com/course/?type=Node.js

* [Facebook 最热门的开源项目推荐！](https://www.itcodemonkey.com/article/1293.html)
* [WebSocket：5分钟从入门到精通](http://mp.weixin.qq.com/s?__biz=MjM5NTEwMTAwNg==&mid=2650213647&idx=1&sn=70467e0ff23500e0498c8fc21775d96e&chksm=befe0d2e8989843883321dbd9c3699218af1f8d4fa1fdbc7560fde9eb985309ab89df386a870&mpshare=1&scene=23&srcid=0108AEvqPGC8sson91HyRNSi#rd)

* [Node.js 原生开发入门完全教程（上）](http://mp.weixin.qq.com/s?__biz=MjM5NTEwMTAwNg==&mid=2650210826&idx=1&sn=230b49e75eaa6ad866174298a33dfdc5&chksm=befe022b89898b3d406e42202fb3f2f8fb863c6ff2b720e25b329969d8a5a2db339ed1a6cd6e&scene=21#wechat_redirect)
* [nodejs api v8.9.3 文档](http://nodejs.cn/api/)

* [阮一峰 nodejs 教程](http://javascript.ruanyifeng.com/nodejs/assert.html)
* [带你入门Nodejs](https://nodelover.me/course/nodejs)
* node modules: https://github.com/node-modules


学习 node module ：https://github.com/parro-it/awesome-micro-npm-packages

* candybox:https://candy.one/i/1205413

* 轻量级实时 Node.js 内核性能监控分析工具 http://easy-monitor.cn/index

>>> 使用NPM下载和发布代码时都会接触到版本号。NPM使用语义版本号来管理代码，这里简单介绍一下。

    语义版本号分为X.Y.Z三位，分别代表主版本号、次版本号和补丁版本号。当代码变更时，版本号按以下原则更新。

    + 如果只是修复bug，需要更新Z位。

    + 如果是新增了功能，但是向下兼容，需要更新Y位。

    + 如果有大变动，向下不兼容，需要更新X位。

* Node提供以下几个全局对象
  ```
    global：表示Node所在的全局环境，类似于浏览器的window对象。需要注意的是，如果在浏览器中声明一个全局变量，实际上是声明了一个全局对象的属性，比如var x = 1等同于设置window.x = 1，但是Node不是这样，至少在模块中不是这样（REPL环境的行为与浏览器一致）。在模块文件中，声明var x = 1，该变量不是global对象的属性，global.x等于undefined。这是因为模块的全局变量都是该模块私有的，其他模块无法取到。

    process：该对象表示Node所处的当前进程，允许开发者与该进程互动。

    console：指向Node内置的console模块，提供命令行环境中的标准输入、标准输出功能。
  ```
  
* Node还提供一些全局函数。
  ```
  setTimeout()：用于在指定毫秒之后，运行回调函数。实际的调用间隔，还取决于系统因素。间隔的毫秒数在1毫秒到2,147,483,647毫秒（约24.8天）之间。如果超过这个范围，会被自动改为1毫秒。该方法返回一个整数，代表这个新建定时器的编号。
  clearTimeout()：用于终止一个setTimeout方法新建的定时器。
  setInterval()：用于每隔一定毫秒调用回调函数。由于系统因素，可能无法保证每次调用之间正好间隔指定的毫秒数，但只会多于这个间隔，而不会少于它。指定的毫秒数必须是1到2,147,483,647（大约24.8天）之间的整数，如果超过这个范围，会被自动改为1毫秒。该方法返回一个整数，代表这个新建定时器的编号。
  clearInterval()：终止一个用setInterval方法新建的定时器。
  require()：用于加载模块。
  Buffer()：用于操作二进制数据。
  ```
* Node提供两个全局变量，都以两个下划线开头。
  ```
  __filename：指向当前运行的脚本文件名。
  __dirname：指向当前运行的脚本所在的目录。
  ```

* 核心模块

```
http：提供HTTP服务器功能。
url：解析URL。
fs：与文件系统交互。
querystring：解析URL的查询字符串。
child_process：新建子进程。
util：提供一系列实用小工具。
path：处理文件路径。
crypto：提供加密和解密功能，基本上是对OpenSSL的包装。
```
