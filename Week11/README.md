学习笔记

简单选择器：
* 通用选择器
div 类型选择器
. class选择器
# id选择器
[attr=value] 属性选择器
Note：包括class选择器和id选择器
:hover 伪类选择器
::before 伪元素选择器

复合选择器
<简单选择器><简单选择器><简单选择器>
*或者div必须写在前面

复杂选择器
<复合选择器><sp><复合选择器>
<复合选择器>">"<复合选择器>
<复合选择器>"~"<复合选择器>
<复合选择器>"+"<复合选择器>
<复合选择器>"||"<复合选择器>

选择器优先级：
选择器优先级=对简单选择器计数
①、!important的优先级是最高的，但出现冲突时则需比较”四位数“;
②、优先级相同时，则采用就近原则，选择最后出现的样式;
③、继承得来的属性，其优先级最低;
-->Note: !important > 行内样式>ID选择器 > 类选择器 > 标签 > 通配符 > 继承 > 浏览器默认属性

伪类：
连接/行为
:any-link
:link-visited
:hover
:active
:focus
:target
树结构
:empty
:nth-child()
:nth-last-child()
:first-child :last-chiild :only-child
逻辑类
:not伪类
:where :has

伪元素：
::before
::after
::first-line
::first-letter