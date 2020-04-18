### for-in和for-of的区别
- for-in循环是遍历键，for-of循环是遍历值
- 遍历对象的时候建议for-in，遍历数组的时候建议for-of
- for-of循环是es6的新增语法。一个数据结构只要部署了Symbol.iterator属性，就被视为具有 iterator 接口，就可以用for...of循环遍历它的成员。也就是说，for...of循环内部调用的是数据结构的Symbol.iterator方法。
```
在实际开发中我们一般在ajax请求中用`不变的html${变量}html标签`代替以前传统复杂的单引号双引号与+的拼接，简介明了，非常好用。

for(let index in aArray){
    console.log(`${aArray[index]}`);
}

for-of
for(var value of aArray){
    console.log(value);
}
```
