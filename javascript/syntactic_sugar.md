# 语法糖

### 1.对象字面量

```text
let a = 'a', b = ‘b’
let c = {a,b}  
```

### 2.箭头函数

```text
let example = function(params){}
可以缩写成 箭头函数会改变this的指向
let example = params =>{}
当参数有两个及以上时
let example = (params1,params2,,,)=>{}
```

### 3.数组解构

```text
let array = ['a','b','c'];
let {a,b} = array
console.log(a) // a
数组解构也允许你跳过你不想用到的值，在对应地方留白即可
let {a,,c} = array
console.log(c)  //c
```

### 4.函数默认参数

```text
function  getData(a,b=0) {}
```

### 5.拓展运算符

```text
function test() {
  return [...arguments]
}
test('a', 'b', 'c') // ['a','b','c']
扩展符还可以拼合数组
 let all = ['1',...['2','3'],...['4','5'],'6']   // ["1", "2", "3", "4", "5", "6"]
```

参考链接：[https://www.jianshu.com/p/bc2e172cb322](https://www.jianshu.com/p/bc2e172cb322)

