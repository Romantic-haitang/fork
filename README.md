```javascript
# fork
双链科技面试题
const getMaxValue=(valueList)=>{
 try {
  
  if (valueList.constructor !== Array ) throw "该数据类型不是数组"
  
  /**
   *  返回最大值 使用ES6的扩展运算符
   */
  // return Math.max(...valueList)
  
  /**
   *  返回最大值 使用 Math 中的 max/min 方法
   */
  // return Math.max.apply(null, valueList);
  
  /**
   * 返回最大值 假设法
   */
  // let max = arr[0];
  
  // for(let i = 1; i < arr.length; i++) {
  //    let cur = arr[i];
  //    cur > max ? max = cur : null
  // }
  // return max
  
  /**
   *  返回最大值 排序法
   */
  
  return valueList.sort((a,b) => a-b)[0]
 } catch (e) {
  console.log(`获取最大数报错信息:${ e }`)
 }
}
export getMaxValue;                          //最后返回模块绑定的函数
```
