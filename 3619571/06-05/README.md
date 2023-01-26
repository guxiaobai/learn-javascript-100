# 05_(掌握)arguments转成array类型

> `2:21:19`


|本期版本|上期版本
|:---:|:---:
`Fri Jan 20 21:56:15 CST 2023` | -


```javascript

arguments.callee

Array.prototype.slice.call(arguments)
[].slice.call(arguments)

// ES6
Array.from(arguments)
[...arguments]
```