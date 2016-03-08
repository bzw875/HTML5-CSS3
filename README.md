# HTML5和CSS3初探
之前的技术分析会，我的主题是HTML5和CSS3，整理出来分享一下

### 维基百科的定义
HTML5是HTML下一个主要的修订版本，现在仍处于发展阶段。目标是取代1999年所制定的HTML 4.01和XHTML 1.0标准，以期能在互联网应用迅速发展的时候，使网络标准达到符合当代的网络需求。广义论及HTML5时，实际指的是包括HTML、CSS和JavaScript在内的一套技术组合。它希望能够减少浏览器对于需要插件的丰富性网络应用服务（plug-in-based rich internet application，RIA)，如Adobe Flash、Microsoft Silverlight，与Oracle JavaFX的需求，并且提供更多能有效增强网络应用的标准集。
具体来说，HTML5添加了许多新的语法特征，其中包括&lt;video&gt;,&lt;audio&gt;,和&lt;canvas&gt;元素，同时集成了SVG内容。这些元素是为了更容易的在网页中添加和处理多媒体和图片内容而添加的。其它新的元素包括&lt;section&gt;, &lt;article&gt;, &lt;header&gt;, 和&lt;nav&gt;,是为了丰富文档的数据内容。新的属性的添加也是为了同样的目的。同时也有一些属性和元素被卸载掉了。一些元素，像&lt;a&gt;, 和&lt;menu&gt;被修改，重新定义或标准化了。同时APIs和DOM已经成为HTML5中的基础部分了。HTML5还定义了处理非法文档的具体细节，使得所有浏览器和客户端程序能够一致地处理语法错误。

### 兼容IE8浏览器
html5shiv.js 让 IE6、IE7、IE8认出 HTML5标签
针对IE浏览器比较好的解决方案是html5shiv。html5shiv主要解决HTML5提出的新的元素不被IE6-8识别，这些新元素不能作为父节点包裹子元素，并且不能应用CSS样式。让CSS 样式应用在未知元素上只需执行 document.createElement(elementName) 即可实现。html5shiv就是根据这个原理创建的。
#####  Respond.js
Respond.js 是一个快速、轻量的 polyfill，用于为 IE6-8 以及其它不支持 CSS3 Media Queries 的浏览器提供媒体查询的 min-width 和 max-width 特性，实现响应式网页设计（Responsive WebDesign）。
html5shiv的使用非常的简单，考虑到IE9是支持html5的，所以只需要在页面head中添加如下代码即可：

```
<!--[if lt IE9]>
<script type="text/javascript" src="//cdn.bootcss.com/html5shiv/3.7.2/html5shiv.min.js"></script>
<script src="//cdn.bootcss.com/respond.js/1.4.2/respond.min.js">/script>
<![endif]-->
```

##### 禁用IE的兼容模式
```<meta http-equiv="X-UA-Compatible" content="IE=edge">```


### HTML5 新标签
* &lt;header&gt;定义文档的头部信息
* &lt;nav&gt;定义导航链接部分
* &lt;footer&gt; 标签定义文档的版权信息
* &lt;section&gt;标签定义文档中的节、区段。比如章节、页眉、页脚或文档中的其他部分。
* &lt;article&gt;定义外部内容（外部链接内容、第三方数据）
* &lt;video&gt;定义视频播放组件
* &lt;command&gt; 标签定义命令按钮，比如单选按钮、复选框或按钮。
* &lt;time&gt; 标签定义日期或时间，或者两者。
* &lt;progress&gt; 标签定义运行中的进度（进程）。
* &lt;meter&gt; 标签定义度量衡。仅用于已知最大和最小值的度量（换言之就是把数字显示成条形图，一目了然原来它们大小差别是这样啊）。
* &lt;aside&gt; 标签定义 article 以外的内容。aside 的内容应该与 article 的内容相关。
* &lt;canvas&gt; 元素用于在网页上绘制图形（非常强大的功能，后面讲到）。
* &lt;command&gt; 标签定义命令按钮，比如单选按钮、复选框或按钮（还不知道怎么用呢...）
* &lt;details&gt; 标签用于描述文档或文档某个部分的细节
* &lt;embed&gt; 标签定义嵌入的内容，比如插件（Flash）。
* &lt;figure&gt; 标签规定独立的流内容（图像、图表、照片、代码等等）。
* &lt;hgroup&gt; 标签用于对网页或区段（section）的标题进行组合。
* &lt;mark&gt; 标签定义带有记号的文本。请在需要突出显示文本时使用 &lt;m&gt; 标签。
* &lt;output&gt; 标签定义不同类型的输出，比如脚本的输出。

### 废除的元素
&lt;acronym&gt;、&lt;applet&gt;、&lt;basefont&gt;、&lt;big&gt;、&lt;center&gt;、&lt;dir&gt;、&lt;font&gt;、&lt;frame&gt;、 &lt;s&gt;、&lt;isindex&gt;、&lt;noframes&gt;、 &lt;frameset&gt; 、&lt;strike&gt;、&lt;tt&gt;、&lt;u&gt;和&lt;xmp&gt;。
