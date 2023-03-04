# 03_(理解)理解柯里化的过程和代码结构

> `00:57:44`


|本期版本|上期版本
|:---:|:---:
`Thu Mar  2 10:30:52 CST 2023` | -

```javascript
function add(x,y,z){
  return x + y +z
}

function sum1(x){
  return function(y){
    return function(z){
      return x + y +z
    }
  }
}

var sum2 = x => y => z =>{
  return x + y + z
}

var sum3 = x => {
  return y => {
    return  z => {
      return  x + y +z
    }
  }
}
```