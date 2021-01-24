学习笔记
了解浏览器的渲染流程：
URL--HTTP-->HTML--parse-->DOM--css computing-->DOM with css--layout-->
DOM with position--render-->Bitmap

状态机：
有限状态机：
每一个状态都是一个机器，有限状态机中的每一个机器都是互相解耦的，在有限状态机中，
每一个机器里可以做计算、存储、输出······
每一个机器知道下一个状态，
每一个机器都有确定的下一个状态--（Moore），
每个机器根据输入决定下一个状态（接收不同的输入，进入不同的状态）（Mealy）。

网络层模型：
ISO-OSI：
物理层、数据链路、网络层、传输层、会话层、表示层、应用层

HTTP response

status line：（HTTP协议版本号、状态码、状态文本）

HTTP状态码：
500系列：服务器内部错误
404：找不到网页
200：OK
301/302/304
header：
body：
