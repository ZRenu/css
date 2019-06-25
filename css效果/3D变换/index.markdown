# transform 

## translate(x,y)定义2D转换
## translate3d(x,y,z)定义3D转换

transform属性应用于元素的2D或3D转换,可以给给定的元素实现旋转（rotate）、缩放（scale）、倾斜（skew）或平移（translate）等。

### translateX()函数表示在二维平画上水平方向移动元素

#### 语法: translateX(t) t:代表了向量平移横坐标的长度

注意： translateX(tx)等同于 translate(tx, 0) 或者 translate3d(tx, 0, 0)。

### translateY()函数表示在页面垂直移动元素

#### 语法: translateY(t)

### translateZ() 定位定义3D转换，用于Z轴，其指定元素向内或向外移动多远。

#### 语法:translateZ（TZ）

tz 表示正值将元素移向观察者，而负值移动远离观察者。


## scale(x[,y]?) 定义 2D 缩放转换
## scale3d(x,y,z) 定义 3D 缩放转换

### scaleX(x) 通过设置 X 轴的值来定义缩放转换。
### scaleY(y) 通过设置 Y 轴的值来定义缩放转换。
### scaleZ(z)  通过设置 Z 轴的值来定义 3D 缩放转换。

## scale取值

单一数值:单一的数值即指定了一个缩放系数，同时作用于X轴和Y轴让该元素进行缩放，相当于指定了单个值的scale()(2D缩放)函数。

两个长度/百分比值:两个数值即分别指定了2D比例的X轴和Y轴的缩放系数，相当于指定了两个值的scale()（2D缩放）函数。

三个长度/百分比值: 三个数值即分别指定了3D比例的X轴、Y轴和Z轴的缩放系数. 相当于一个scale3d()函数。

none:指定不进行缩放。

## rotate(angle) 定义 2D 旋转，在参数中规定角
## rotate3d(x,y,z,angle) 定义 3D 旋转。

## rotate()函数定义了一种将元素围绕一个定点（由transform-origin属性指定）旋转而不变形的转换。指定的角度定义了旋转的量度。若角度为正，则顺时针方向旋转，否则逆时针方向旋转。旋转180°也被称为点反射

元素旋转的固定点 - 如上所述 - 也称为变换原点。这默认为元素的中心，但你可以使用transform-origin属性设置自己的自定义变换原点。

### rotateX(angle) 定义沿着 X 轴的 3D 旋转。
### rotateY(angle) 定义沿着 Y 轴的 3D 旋转
### rotateZ(angle) 定义沿着 Z 轴的 3D 旋转。


## skew(x-angle,y-angle) 定义沿着 X 和 Y 轴的 2D 倾斜转换
### skewX(angle) 定义沿着 X 轴的 2D 倾斜转换。
### skewY(angle) 定义沿着 Y 轴的 2D 倾斜转换。

## perspective 为3D转换元素定义透视视图。

## transform-origin CSS属性让你更改一个元素变形的原点。

### 语法: transform-origin: x-axis y-axis z-axis;

left(0%) | center(50%) | right(100%) | top(0%) | bottom(100%)

x-axis: 定义视图被置于 X 轴的何处 left center right lenght %
y-axis: 定义视图被置于 Y 轴的何处 top center bottom length %
z-axis: 定义视图被置于 Z 轴的何处。可能的值：length


## transform--style 属性指定嵌套元素是怎样在三维空间中呈现。
>* flat 表示所有子元素在2D平面呈现。
>* preserve-3d 表示所有子元素在3D空间中呈现。