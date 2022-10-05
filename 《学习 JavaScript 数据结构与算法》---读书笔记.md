# 数组

1. Array.from 方法根据已有的数组创建一个新数组, 实现数据 copy

2. 数组中有三个能够获得迭代器的方法: entries keys 和 values. 得到的数组能够通过 next() 获取数组中下一组数据

3. 自定义排序

   ```js
   // 对象数组的排序
   const friends = [
     {name: 'John', age:30},
     {name:'Ana', age:20},
     {name:'Chris', age:25}
   ]
   function comparePerson(a, b){
     if(a.age < b.age){
       return -1
     }
     if(a.age > b.age){
       return 0
     }
     return 0
   }
   console.log(friends.sort(comparePerson)) 
   // 输出
   [
       {"name": "Ana","age": 20},
       {"name": "Chris","age": 25},
       {"name": "John","age": 30}
   ]
   ```

   

