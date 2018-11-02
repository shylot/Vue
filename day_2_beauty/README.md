# day_2_beauty
本项目为升级版，

## 一、过度类名
### 1.1 v-enter
定义进入过渡的开始状态。在元素被插入之前生效，在元素被插入之后的下一帧移除。
### 1.2 v-enter-active
定义进入过渡生效时的状态。在整个进入过渡的阶段中应用，在元素被插入之前生效，在过渡/动画完成之后移除。这个类可以被用来定义进入过渡的过程时间，延迟和曲线函数。
### 1.3 v-enter-to
`v2.1.8及以上`版本中定义进入过渡后的结束状态。在元素被插入之后下一帧生效（与此同时```v-enter```被移除），在过渡/动画完成之后移除。
### 1.4 v-leave
定义离开过渡的开始状态。在离开过渡被触发时立刻生效，下一帧被移除。
### 1.5 v-leave-active
定义离开过渡生效时的状态。在整个离开过渡的阶段中应用，在离开过渡被触发时立刻生效，在过渡/动画完成之后移除。这个类可以被用来定义离开过渡的过程时间，延迟和曲线函数。
### 1.6 v-leave-to
`v2.1.8及以上`版本中定义离开过渡后的结束状态。在离开过渡被触发之后下一帧生效（与此同时`v-leave`被删除），在过渡/动画完成之后移除。

## 二、CSS3动画
### 2.1 transition
`语法` `transition: property duration timing-function delay`

过渡。允许CSS的属性值在一定的时间内平滑的过渡。这种效果可以在`鼠标单击`、`获得焦`点或`元素任何改变`中触发，并圆滑地以动画效果改变CSS属性值。
  
#### 2.1.1 property
规定设置过渡效果的CSS属性名称。如`background`、`left`等等
#### 2.1.2 duration
定义动画时间，`默认0`。如`1s`、`10ms`等等
#### 2.1.3 timing-function
定义速度函数，`默认ease`


- linear `相同的速度开始至结束（等于cubic-bezier(0,0,1,1)）`
- ease `慢速开始，然后变快，最后慢速结束（等于cubic-bezier(0.25,0.1,0.25,1)）`
- ease-in `慢速开始（等于cubic-bezier(0.42,0,1,1)）`
- ease-out `慢速结束（等于cubic-bezier(0,0,0.58,1)）`
- ease-in-out `慢速开始至结束（等于cubic-bezier(0.42,0,0.58,1)）`
- cubic-bezier(n,n,n,n) `自定义贝塞尔曲线，取值[0,1]`
- steps `步骤次数，[start/end]`

#### 2.1.4 delay
定义动画效果何时开始（将过渡效果推迟多久），`默认0`

### 2.2 transform
`语法` `transform: none|transform-funciton`

转换。向元素应用2D或3D转换。该属性允许对元素进行`旋转`、`缩放`、`移动`或`倾斜`

#### 2.2.1 matrix
矩阵转换
- matrix(n,n,n,n,n,n) `2D转换，使用六值的矩阵`
- matrix3D(n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n) `3D转换，使用十六值的4X4矩阵`
#### 2.2.2 translate
坐标轴转换
- translate(x,y) `2D转换`
- translate3d(x,y,z) `3D转换`
- translateX(x) `转换，只用X轴的值`
- translateY(y) `转换，只用Y轴的值`
- translateX(z) `3D转换，只用Y轴的值`
#### 2.2.3 scale
 缩放转换
- scale(x,y) `2D缩放`
- scale3d(x,y,z) `3D缩放`
- scaleX(x) `X轴缩放`
- scaleY(y) `Y轴缩放`
- scaleZ(z) `3D转换，Z轴缩放`
#### 2.2.4 rotate
 旋转转换
- rotate(deg) `2D旋转`
- rotate(x,y,z,deg) `3D旋转`
- rotate(deg) `X轴旋转`
- rotate(deg) `Y轴旋转`
- rotate(deg) `3D转换，Z轴旋转`
#### 2.2.5 skew
倾斜转换
- skew(x-deg,y-deg) `2D转换，沿着X轴、Y轴倾斜`
- skewX(deg) `沿着X轴倾斜`
- skewY(deg) `沿着Y轴倾斜`
#### 2.2.6 perspective
透视视图转换
- perspective(n) `3D转换`

### 2.3 animation
`语法` `name duration timing-function delay iteration-count direction`

动画
#### 2.3.1 name
绑定到选择器`keyframe`名称
#### 2.3.2 duration
动画持续时间，单位`s`或`ms`
#### 2.3.3 timing-function
动画将如何完成一个周期
#### 2.3.4 delay
动画开始之前的延迟时间
#### 2.3.5 iteration-count
播放次数
#### 2.3.6 direction
是否轮流反向播放动画
- normal `默认，正常播放`
- reverse `反向播放`
- alternate `动画在奇数次正向播放，偶数次反向播放`
- alternate-reverse `动画在奇数次反向播放，偶数次正向播放`
- initial `默认`
- inherit `从父类继承`


 
