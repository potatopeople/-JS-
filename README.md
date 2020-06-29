# 个人练习JS、CSS时做的一些小东西，喜欢的话可以拿去使用。

## 日期选择器:
用原生JS制作的一个日期选择器模块，支持外部引入调用。
> * 点击年或月份元素，弹出输入框，自定义输入年份和月份(使用了正则进行处理)，回车键确定。
> * 点击号数进行日期的切换，切换完成后点击下方的确定按钮会确定日期，点击取消的话会重置为上次确认的日期值。
```
//引入2个样式文件
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.0.0/animate.min.css">
 <link rel="stylesheet" href="./index.css">
 
 //内容容器和日期盒子
 <input style="font-size:18px;text-align:center;" id="date-text" />
 <div class="date-box"></div>
 
 //引入日期js文件
 <script src="./index.js"></script>
 
    //存放日期的容器
    const contentBox = document.getElementById('date-text')
    //日期元素外层盒子
    const dateBox = document.getElementsByClassName('date-box')[0]

    /*
    **初始化实例,需要传入：存放日期的容器，日期元素盒子，一个初始化时间，点击确定和取消按钮后是否要隐藏(默认为否)
    **选择时间后，可以通过dateFn.year，dateFn.month + 1，dateFn.day 拿到年月日时间
    */
    const dateFn = new DateReterFace(contentBox,dateBox,new Date(),true)
```
## 图片控制：
对于图片的放大、缩小、旋转、拖动。

## 图片闪烁：
>鼠标移入图片有白光闪过。

## 翻页效果：
>翻页动画

## 球体：
>CSS制作的一个球体

## 人员抽签：
>对一组人员数据按输入的数字，进行随机抽取。