###transition
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
[过渡demo](http)
