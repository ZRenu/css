# css动画

## 动画类型

>* transition补间动画
>* animations keyframe关键帧动画
>>* 逐帧动画：逐帧动画属于关键帧动画特殊用法，适用于无法补间计算的动画，资源较大使用steps()

## transition 

过渡可以为一个元素在不同状态之间切换的时候定义不同的过渡效果。比如在不同的伪元素之间切换，像是 :hover，:active 或者通过 JavaScript 实现的状态变化。

transition属性可以被指定为一个或多个 CSS 属性的过渡效果，多个属性之间用逗号进行分隔。

>* transition-property 指定应用过渡属性的名称
>* transition-duration 属性以秒或毫秒为单位指定过渡动画所需的时间。默认值为 0s ，表示不出现过渡动画。
>* transition-timing-function 指定切换效果的速度
>>* linear 规定以相同速度开始至结束的过渡效果
>>* ease 规定慢速开始，然后变快，然后慢速结束的过渡效果
>>* ease-in 规定以慢速开始的过渡效果
>>* ease-out 规定以慢速结束的过渡效果
>>* ease-in-out 规定以慢速开始和结束的过渡效果
>* transition-delay 规定了在过渡效果开始作用之前需要等待的时间。

### 语法  transition: property duration timing-function delay

## animations 可以将从一个CSS样式配置转换到另一个CSS样式配置。动画包括两个部分:描述动画的样式规则和用于指定动画开始、结束以及中间点样式的关键帧。

### animation的子属性有:
>* animation-delay 设置延时，即从元素加载完成之后到动画序列开始执行的这段时间
>* animation-direction 设置动画在每次运行完后是反向运行还是重新回到开始位置重复运行。
>* animation-duration 设置动画一个周期的时长。
>>* normal 每个循环内动画向前循环，换言之，每个动画循环结束，动画重置到起点重新开始，这是默认属性。
>>* alternate 动画交替反向运行，反向运行时，动画按步后退，同时，带时间功能的函数也反向，比如，ease-in 在反向时成为ease-out。计数取决于开始时是奇数迭代还是偶数迭代
>>* reverse 反向运行动画，每周期结束动画由尾到头运行。
>>* alternate-reverse 反向交替， 反向开始交替
>* animation-iteration-count 设置动画重复次数， 可以指定infinite无限次重复动画
>* animation-name 指定由@keyframes描述的关键帧名称。
>* animation-play-state 允许暂停和恢复动画。
>>* running 当前动画正在运行。
>>* paused 当前动画以被停止。
>* animation-timing-function 设置动画速度， 即通过建立加速度曲线，设置动画在关键帧之间是如何变化
>* animation-fill-mode  指定动画执行前后如何为目标元素应用样式。

#### keyframes定义动画序列

一旦完成动画的时间设置， 接下来就需要定义动画的表现。通过使用@keyframes建立两个或两个以上关键帧来实现。每一个关键帧都描述了动画元素在给定的时间点上应该如何渲染。

因为动画的时间设置是通过CSS样式定义的，关键帧使用percentage来指定动画发生的时间点。0%表示动画的第一时刻，100%表示动画的最终时刻。因为这两个时间点十分重要，所以还有特殊的别名：from和to。这两个都是可选的，若from/0%或to/100%未指定，则浏览器使用计算值开始或结束动画。

也可包含额外可选的关键帧，描述动画开始和结束之间的状态。

## 语法 animation: name duration timing-function delay iteration-count direction;


## 动画事件

利用动画事件可以更好的控制动画和信息。这些事件由 AnimationEvent对象表示，可探测动画何时开始结束和开始新的循环。每个事件包括动画发生的时间和触发事件的动画名称。