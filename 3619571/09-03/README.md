# 03_(掌握)创建对象方案-工厂模式

> `2:27:19`


|本期版本|上期版本
|:---:|:---:
`Sun Jan 29 01:25:38 CST 2023` | -



```javascript

function createPerson(name)
{
	var p = {}
	p.name = name
	return p
}

var p1 = createPerson('a')
var p1 = createPerson('p')
```

* 没有类型(获取不到对象真实的类型)
* 