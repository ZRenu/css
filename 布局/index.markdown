# 布局

>* 表格
>* float + margin
>* inline-block
>* flexbox

## 盒模型

<img src='../布局/1.png'>

## display/position

>* 确定元素的显示类型 display: block/inline/inline-block
>* 确定元素的位置 static/relative/absolute/fixed
>>* static
>>* relative 相对定位，相对于自身
>>* absolute 绝对定位，脱离文档流，相对于body或者最近的relative或者absolute
>>* fixed 绝对定位，脱离文档流，相对屏幕的可视区域


## z-index

## flexbox布局

>* 弹性盒子
>* 盒子本来就是并列
>* 指定宽度即可

## float布局

>* 元素浮动
>* 脱离文档流，不脱离文本流
>* 对自身的影响:
>>* 形成‘块’（BFC）
>>* 位置尽量靠上
>>* 位置尽量靠左（右）
>* 对兄弟元素的影响：
>>* 上面贴非float元素
>>* 旁边贴float元素
>>* 不影响其他块级元素位置
>>* 影响其它块级元素内部文本
>* 对父级的影响:
>>* 从布局上‘消失’
>>* 高度塌陷

## inline-block布局

>* 像文本一样排block元素
>* 没有清楚浮动等问题
>* 需要处理间隙

## 响应式布局

>* 在不通设备上正常使用
>* 一般主要屏幕大小问题
>* 主要方法:
>>* 不同设备独立的设计方案
>>* 隐藏 + 折行 + 自适应空间
>>* rem / viewport / media query



