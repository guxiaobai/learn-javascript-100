# 03_(掌握)多个绑定规则优先级比较

> `44:22`


|本期版本|上期版本
|:---:|:---:
`Fri Jan 20 21:56:15 CST 2023` | -


* 显示绑定高于隐式绑定
* new 的优先级高于隐式绑定

```javascript
function foo(){
	console.log(this)
}

var obj = {
	name: 'obj',
	foo: foo.bind('aa')
}

obj.foo()
```
