学习笔记
表达式：

语法树和运算符优先级

语法树与运算符优先级的关系

运算符优先级会影响到语法树的构成

运算符优先级（由高到低）

Member：

--a.b

--a[b]

--foo `string`

--super.b

--super['b']

--new.target

--new Foo()

Call:

--foo()

--super()

--foo()['b']

--foo().b

--foo()`abc`

Left Handside & Right Handside

--a.b = c

Unary

--delete a.b

--void foo()

--typeof a

--+a

---a

--~a

--!a

--await a

Multiplicative

-- * / %

-- Additive + -

-- Shift(移位运算) <<  >> >>>

-- Relationship < > <=  >=

Equality

-- ==

-- !=

-- ===

-- !==

Bitwise

-- & ^ |

Logical

-- &&

-- ||

Conditional

--?

类型转换：

a+b （前提a,b类型不是Number，String）

运行时的相关概念：

语句：Completion Record

[[type]]: normal, break, continue, return, or throw

[[value]]: 基本类型

[[target]]: label

语句：

简单语句

表达式语句

空语句

deBugger语句

throw语句

continue语句

break语句

return语句

复合语句

BlockStatement

IfStatement

SwitchStatement（不建议在JavaScript中使用）

IterationStatement

WithStatement

LabelledStatement（再简单语句或者复合语句前加上一个名字）

TryStatement--try{}catch()finally()



