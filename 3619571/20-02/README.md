# 02_(掌握)Promise-对象方法-then方法

> `25:10`


|本期版本|上期版本
|:---:|:---:
`Wed Feb  1 17:09:42 CST 2023` | -



* 同一个 Promise 可以被多次调用 then 方法 
* 所有的 then 方法都会被调用


### then 方法的回调函数可以有返回值

* 返回一个普通的值，那么这个普通的值被作为一个新的Promise的 `resolve`的值


```javascript
promise.thne(res=>{
	return {name: 'guxiaobai'}
	// return undefined
}).then(res=>{
	console.log(res.name)
})