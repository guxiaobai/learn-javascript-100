# 08_(掌握)全局代码执行和作用域提升

> `2:13:10`


|本期版本|上期版本
|:---:|:---:
`Sat Jan 28 23:50:56 CST 2023` | -


* js引擎会在执行代码之前，会在堆内存中创建一个全局对象：`Global Object（GO）`
* js引擎内部有一个执行上下文栈（`Execution Context Stack，简称ECS`）
* 全局的代码块为了执行会构建一个 `Global Execution Context（GEC）`
* 一个函数执行上下文（`Functional Execution Context，简称FEC`）


## FEC中包含三部分内容

* 第一部分：在解析函数成为AST树结构时，会创建一个`Activation Object（AO）`
	* 包含形参、arguments、函数定义和指向函数对象、定义的变量；
* 第二部分：作用域链：由VO（在函数中就是AO对象）和父级VO组成，查找时会一层层查找；
* 第三部分：this绑定的值：这个我们后续会详细解析；


## Misc

* 在GCE中VO就是GO