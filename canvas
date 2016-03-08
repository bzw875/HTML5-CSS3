```
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>canvas绘图</title>
</head>

<body>
<canvas id="canvas" width="300" height="300"></canvas>
<script>
var canvas = document.getElementById("canvas");
// 从canvas获取二维环境
var ctx = canvas.getContext("2d");
// 绘制填充矩形起点坐标x:20,y:25；width:150,height:100
ctx.fillRect(20, 25, 150, 100);
// 创建一个新的路径
ctx.beginPath();
// 绘制圆弧路径圆心坐标x:220,y:110;半径:100;圆弧的起始点(Math.PI * 1/2)弧度;圆弧的终点(Math.PI * 3/2)弧度
ctx.arc(220, 110, 100, Math.PI * 1/2, Math.PI * 3/2);
// 路径宽度
ctx.lineWidth = 15;
// 线段末端属性为以圆形结束
ctx.lineCap = 'round';
// 画笔颜色为rgba(255, 127, 0, 0.5)色
ctx.strokeStyle = 'rgba(255, 127, 0, 0.5)';
// 绘制当前或已经存在的路径的方法
ctx.stroke();
</script>
</body>
</html>
```
