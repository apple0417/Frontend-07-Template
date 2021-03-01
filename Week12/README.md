学习笔记
盒（Box）
1.区分标签、元素、盒之间的区别
HTML代码中可以书写开始标签、结束标签、自封闭标签
一对起止标签表示一个元素
DOM树中存储的是元素和其他类型的节点（元素是节点的一种）
CSS选择器中的是元素（或者伪元素）
CSS选择器选中的元素，在排版时可能会产生多个盒
排版和渲染的基本单位是盒
2.盒模型
content  padding  border  margin
box-sizing：content-box   border-box

CSS的排版-->字、盒
1.正常流
（从左到右，满行换下一行，每行对齐）
如果是文字，收进盒中
对一行中的盒进行排版
对行进行排版
行内：IFC（行内级格式化上下文，从左到右）
块级：BFC（块级格式化上下文， 从上到下）

正常流的行级排布(默认基线对其规则)：
line-top
text-top
base-line
text-bottom
line-bottom
Note：inline-block中的基线随着文字改变，可以加对其方式：vertical-align: top/middle/bottom/text-top/text-bottom

正常流的块级排布：
1.float和clear
float浮动元素：脱离正常流
clear和float结合可以实现绕排
2.margin堆叠
前一个盒模型与后一个盒模型之间如果分别设置margin-bottom和margin-top属性，那么会产生margin堆叠，取值为最大margin留白
Note：margin堆叠现象只会出现在BFC中

BFC（块级格式化上下文）合并
Block Container ：里面有BFC
Block-level Box：外面有BFC
Block Box = Block Container + Block-level Box：
里外都有BFC

Flex排版
1.收集盒进行
2.计算盒在主轴方向的排布
3.计算盒在交叉轴上的排布
分行：
1.根据主轴的尺寸，把元素分进行中
2.若设置了top-wrap，则强行分配进第一行
计算主轴方向：
1.找出所有Flex的元素
2.把周周方向的剩余尺寸按比例分配给这些元素
3.若剩余空间为负数，所有flex元素为0，等比例压缩剩余元素
计算交叉轴方向：
1.根据每一行中最大元素尺寸计算行高
2.根据行高flex-align和item-align，确定元素具体位置

Animation
1.animation-name 时间曲线
2.animation-duration 动画的时长
3.animation-timing-function 动画的使劲啊曲线
4.animation-delay 动画开始前的延迟
5.animation-iteration-count 动画的播放次数
6.animation-direction 动画的方向