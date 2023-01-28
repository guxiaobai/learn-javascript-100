# 02_(理解)Object对对象限制的方法补充

> `23:19`


|本期版本|上期版本
|:---:|:---:
`Sun Jan 29 01:21:17 CST 2023` | -


* `Object.getOwnPropertyDescriptor()`

```javascript
// 禁止对象继续添加新的属性
Object.preventExtensition

// 禁止配置
Object.seal

 // 不可修改
 Object.freeze
```