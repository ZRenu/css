# 非布局样式

>* 字体、子重、颜色、大小、行高
>* 背景、边框
>* 滚动、换行
>* 粗体、斜体、下划线
>* 其他

## 行高

### 行高的构成

inline box的高度会决定行高的高度

### 行高的相关现象和方案

>* 图片下面为什么会有空隙？解决？

因为img的display的默认值inline，就会涉及到字体对齐，默示是baseline,baseline和底线（bottom）之间会存在偏差，偏差大小视字体大小而定。

解决: 
```css
vertical-align:bottom;
```

### 行高的调整

## 背景

>* 背景颜色
>* 渐变色背景
>* 多背景叠加
>* 背景图片和属性（雪碧图)
>* base64和性能优化
>* 多分辨率适配

## 边框

>* 线型 大小 颜色
>* 边框图
>* 边框衔接

## 滚动

>* 滚动行为和滚动条
>* > visible 滚动条隐藏，多余内容会溢出容器
>* > hidden  滚动条隐藏，多余内容会隐藏
>* > scroll  滚动条显示
>* > auto    滚动条自动显示

## 文本

### 文本折行
>* overflow-wrap(word-wrap) 通用换行控制
>* word-break 针对多字节的文字
>* white-space 空白处是否断行

## 装饰性属性

>* 粗体 font-weight
>* 斜体 font-style:itaic
>* 下划线: text-decoration
>* 指针: cursor