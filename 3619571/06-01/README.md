# 01_(掌握)自己实现函数的call方法

> `00:00:00`


|本期版本|上期版本
|:---:|:---:
`Wed Mar  1 17:24:17 CST 2023` | -

```javascript
Function.prototype.hycall = function(thisArg， ...args){
  // 1. 获取需要被执行的函数
  var fn = this

  // 2. 对thisArg转成对象类型(防止它传入的是非对象类型)
  thisArg = thisArg ? Object(thisArg) : window

  // 调用需要被执行的函数
  thisArg.fn = fn
  thisArg.fnd()
  delete thisArg.fn
}
```