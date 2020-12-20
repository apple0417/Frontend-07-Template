学习笔记
AST语法树
对于AST语法树的理解
抽象语法树是源代码的抽象语法结构的树状表示，树上的每一个节点都表示源代码中的一种结构，
所以说是抽象的，是因为抽象语法树并不会表示真实语法出现的每一个细节。
案例：四则运算的分析
输入元素（有意义的输入--token）：

词法：

数字（Number）0-9组合（支持带有小数点）

运算符（Operator）加减乘除

LL语法分析语法：

<AdditiveExpression>::=

<Number>

|<MultiplicationExpression><*><Number>

|<MultiplicationExpression></><Number>

|<AdditionExpression><+><MultiplicationExpression>

|<AdditionExpression><-><MultiplicationExpression>

