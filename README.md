## 一个canvas画板 
* 一个用于练习的canvas画板
### 用到的API
1. 创建canvas
```
 <canvas id="canvas" width='100' height='100'></canvas>
```
2. canvas.getContext：
* “2d”,创建一个CanvasRenderingContext2D对象作为2D渲染的上下文。
3. 判断手机触摸还是PC鼠标点击移动
* `var isTouchDevice = 'ontouchstart' in document.documentElement;`
* 如果是手机触摸
    * 调用`canvas.ontouchstart`和`canvas.ontouchmove`
* 如果是PC鼠标事件
    * 调用 `canvas.onmousedown`、 `canvas.onmousedown`、`canvas.onmouseup`
