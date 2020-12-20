---
title: 关于uni-app，uni.request 在ios12版本请求失败的问题
---
 

## 在h5端，微信浏览器及手机自带浏览器

### 出现的问题及报错。
 请求不能成功，请求发不出去，不报其他错误。

``` bash
"errMsg":"request:fail"
```

### 原因
 属于cors的问题，header出现自定义的请求字段，而服务器端Access-Control-Allow-Headers:没有该字段

### 如何解决

 在服务器端Access-Control-Allow-Headers:设置对应客户端请求的字段，就可以解决这个问题，并且这个问题在ios12以下会出现，在其他版本不会出现该问题.