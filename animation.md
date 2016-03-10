###transition过渡
```
<img class="transition-pic" src="images/canvas1.jpg">
<style type="text/css">
.transition-pic {
  width: 100px;
  height: 100px;
  -webkit-transition:width .8s, height .8s, -webkit-transform .8s;
/*
  其实是下面的简写
  transition-duration: .8s; 过渡持续时间
  transition-property: width; 过渡的属性
  ...
*/
}
.transition-pic:hover {
  width: 300px;
  height: 300px;
/*  修改它的可视化模型: 旋转360度 */
  -webkit-transform:rotate(360deg);
}
</style>
```
[过渡demo](http://bzw875.github.io/jekyll_demo/2016/03/09/animation.html#transition)

###keyframes动画

```
<style type="text/css">
.keyframes-div {
    width: 100px;
    height: 100px;
    background: red;
    position: relative;
    /*动画名称myfirst，持续时间:5秒*/
    -webkit-animation: myfirst 5s
}
@-webkit-keyframes myfirst {
    /*百分比是动画持续的时间的百分比*/
    0% {
        background-color: #ff0000;
        left: 0px;
        top: 0px
    }
    25% {
        background-color: #ffff00;
        left: 200px;
        top: 0px;
        border-radius: 25px
    }
    50% {
        background-color: #00ff00;
        left: 200px;
        top: 200px;
        border-radius: 50px
    }
    75% {
        background-color: #ff00ff;
        left: 0px;
        top: 200px;
        border-radius: 25px
    }
    100% {
        background-color: #ff0000;
        left: 0px;
        top: 0px
    }
}
</style>
<div class="keyframes-div"></div>
```

[动画demo](http://bzw875.github.io/jekyll_demo/2016/03/09/animation.html#keyframes)
