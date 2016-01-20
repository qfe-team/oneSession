# oneSession

> 仅存取一次的session, 一般用来做移动端的页面间传值.

> 如果浏览器环境不支持session, 则采用cookie的方式传值. (兼容无痕模式)

## 适用场景:

* 页面执行某项操作, 提示要登录跳转到登录页面. 跳转之前存储原页面的session, 登录操作结束后判断是否存在该session. 如果存在则跳转回来, 否则跳转到用户中心.
* 页面a的值想不通过url的方式传递给页面b, 且该数据不需要长期保留.

## API

```
oneSession.set(key,value);  //存储
oneSession.get(key);        //获取
```
