```javascript
# fork
双链科技面试题



const getMaxValue=(valueList)=>{
 if (!valueList.length) return                    //首先先查询数组的长度 
 valueList.sort((a,b) => a - b) [0]               // 使用sort方法对数组元素进行排序  取下标第一个最大的number
}
export getMaxValue;                               //最后返回模块绑定的函数
```

