# IdCard - 18位身份证的工具
----
本来是不想重新造轮子的可是找了找github上的仓库,看了看感觉都有bug而且很别扭,所以还是自己开刀搞,说说跟别的库有什么不同吧
- 对地区数据上不准备直接用网上的一些数据因为那些数据在计算到县和区的时候会漏掉市级的一些数据所以准备先对数据进行二次处理在引入




## 方法列表
----
### IdCard.EndNum(IdCard)
返回根据前17位数算出来的第18位

##### 参数说明
- @param {Number} IdCard 身份证号码

##### 返回数据
`{Number}`

### IdCard.Birthday(IdCard)
返回计算出来的星期几,星座,生肖

##### 参数说明
- @param {Number} IdCard 身份证号码

##### 返回数据
```js
{
  date: 20010101,
  year: 2001,
  month: 01,
  date: 01,
  week: '星期一', // 星期几
  zodiac: '天秤座',  // 星座
  zodiac_zh: '龙'  // 生肖
}
```
