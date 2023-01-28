# 06_(掌握)对象的原型理解和作用

> `2:27:19`


|本期版本|上期版本
|:---:|:---:
`Sun Jan 29 01:38:57 CST 2023` | -



* `__proto__` / `Object.getPrototypeOf()`
* 隐式原型
* 在当前对象没有找到，就会沿着原型链查找

```javascript
var obj = {}
obj.__proto__.age = 18
obj.age
```