# 05_(掌握)认识面向对象和JS创建对象的方式

> `1:26:19`


|本期版本|上期版本
|:---:|:---:
`Sun Jan 29 00:51:54 CST 2023` | -

* 通过new Object 方式创建


```javascript

var obj = new Object();
obj.name = "why"
obj.running = function(){
	console.log(this.name + "在跑步")
}
```

* 通过字面量形式


```javascript
var obj = {
	name : "why",
	running: function(){
		console.log(this.name + "在跑步")
	}
}
```