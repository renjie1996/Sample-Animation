# Sample-Animation
雪碧图动画
##animation中的steps()：

 `animation: walker 1s steps(5) infinite;`
解释：

###1.steps 是animation 的一种属性，steps(x)，x是指将中间的过程分为x份，忽略掉中间过渡的部分。

animation 中的steps()在animation-timing-function帧进行划分，5帧数5等分，动画只会在这5帧的等分做停留切换，并不会过渡。

###2.雪碧图

包含多帧的图片，采用background-position动画，雪碧图就是将多张图片合并一张图上，有利于减少网络http请求。

###3.做法：from 0 0 to 0 -100%;
