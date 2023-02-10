# 02_(掌握)继承-原型式继承函数的实现

> ``


|本期版本|上期版本
|:---:|:---:
`Fri Jan 20 21:56:15 CST 2023` | -


```javascript
function creatObject(o){
  var newObj = {}
  Object.setPrototypeOf(newObj, o)
  return newObj
} 
```

```javascript
function creatObject(o){
  function Fn() {}
  Fn.prototype = o

  var newObj = new Fn()

  return newObj
}
```

```javascript
Object.create()
```
