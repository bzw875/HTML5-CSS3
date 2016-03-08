之前的技术分析会，我的主题是HTML5和CSS3，整理出来分享一下

## 维基百科的定义

HTML5是HTML下一个主要的修订版本，现在仍处于发展阶段。目标是取代1999年所制定的HTML 4.01和XHTML 1.0标准，以期能在互联网应用迅速发展的时候，使网络标准达到符合当代的网络需求。广义论及HTML5时，实际指的是包括HTML、CSS和JavaScript在内的一套技术组合。它希望能够减少浏览器对于需要插件的丰富性网络应用服务（plug-in-based rich internet application，RIA)，如Adobe Flash、Microsoft Silverlight，与Oracle JavaFX的需求，并且提供更多能有效增强网络应用的标准集。
具体来说，HTML5添加了许多新的语法特征，其中包括<video>,<audio>,和<canvas>元素，同时集成了SVG内容。这些元素是为了更容易的在网页中添加和处理多媒体和图片内容而添加的。其它新的元素包括<section>, <article>, <header>, 和<nav>,是为了丰富文档的数据内容。新的属性的添加也是为了同样的目的。同时也有一些属性和元素被卸载掉了。一些元素，像<a>, 和<menu>被修改，重新定义或标准化了。同时APIs和DOM已经成为HTML5中的基础部分了。HTML5还定义了处理非法文档的具体细节，使得所有浏览器和客户端程序能够一致地处理语法错误。

### 兼容IE8浏览器
html5shiv.js 让 IE6、IE7、IE8认出 HTML5标签
针对IE浏览器比较好的解决方案是html5shiv。html5shiv主要解决HTML5提出的新的元素不被IE6-8识别，这些新元素不能作为父节点包裹子元素，并且不能应用CSS样式。让CSS 样式应用在未知元素上只需执行 document.createElement(elementName) 即可实现。html5shiv就是根据这个原理创建的。
html5shiv的使用非常的简单，考虑到IE9是支持html5的，所以只需要在页面head中添加如下代码即可：

```<!--[if lt IE9]>
<script type="text/javascript" src="scripts/html5shiv.js"></script>
<![endif]-->```

##### 禁用IE的兼容模式
```<meta http-equiv="X-UA-Compatible" content="IE=edge">```


#####  Respond.js
Respond.js 是一个快速、轻量的 polyfill，用于为 IE6-8 以及其它不支持 CSS3 Media Queries 的
浏览器提供媒体查询的 min-width 和 max-width 特性，实现响应式网页设计（Responsive Web
Design）。
