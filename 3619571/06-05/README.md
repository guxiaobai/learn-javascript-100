# 05_(掌握)arguments转成array类型

> `1:52:00`


|本期版本|上期版本
|:---:|:---:
`Wed Mar  1 17:35:29 CST 2023` | -

```javascript
Array.prototype.slice.call(arguments)
[].slice.call(arguments)

// ES6
Array.from(arguments)
[...arguments ]
```