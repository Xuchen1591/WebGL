# WebGL
WebGL learning records

Source: http://blog.csdn.net/column/details/webgl.html?&page=2


>>>
node
	- content


> * 1.


> * 2.


> * 3.


> * 4. 渲染准备

```javascript
    <script id="vshader" type="x-shader/x-vertex">
        ※顶点着色器
    </script>

    <script id="fshader" type="x-shader/x-fragment">
        ※片段着色器
    </script>
```


> * 5.


> * 6. 顶点和多边形
	－ 顶点的连接顺序和遮挡剔除


> * 7. context的设定


> * 8. 着色器的说明和基础
    - GLSL（OpenGL Shading Language）
    - 顶点着色器和片段着色器
    - 顶点着色器就是处理顶点相关的信息，片段着色器就是处理画面上的颜色信息
    - 着色器的内部，必须要定义一个main函数，在这个函数里面添加自己的处理
    - 要向着色器传递各个顶点的不同的信息的时候，使用attribute修饰符声明变量
    - 要向着色器传递对所有顶点来说都一样的信息的时候，使用uniform修饰符声明变量
    - 从顶点着色器向片段着色器传递数据的时候，使用varying修饰符声明变量
    - 顶点着色器中内置的变量gl_Position必须赋值，而片段着色器的内置变量gl_FragColor虽然不是必须赋值的

> * 9. 顶点缓存的基础
    - VBO Vertex Buffer Object
    - VBO的生成需要使用一维数组

    - 顶点的各种信息保存到数组里
    - 使用WebGL的方法生成VBO
    - 使用WebGL的方法将数组中的信息传给VBO
    - 顶点着色器中的attribute函数和VBO结合

    - 使用WebGL的context的方法生成VBO，当然生成的时候VBO是空的，然后将顶点信息的数组传给它

> * 10. 矩阵计算和外部库