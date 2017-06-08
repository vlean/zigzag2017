# 图解HTTP笔记
## 0x00 说明
HTTP 1.1

### OSI七层网络模型 & TCP/IP四层模型
![Alt text](./1099668-20170212153338135-125492424.jpg)

![Alt text](./0_13122714161Qzd.gif)

## 0x03 HTTP报文内的HTTP信息

## 0x04 HTTP状态码

- **1xx 信息性状态码   接受的请求正在处理中**
- **2xx 成功状态码   请求正常处理完毕**
- - 200 请求正常
- - 204 no content 请求处理成功，但没有资源可返回
- - 206 partial content 对一部分资源的请求，响应请求头中Content-Range的范围
- **3xx 重定向状态码 需要进行附加操作已完成请求**
- - 301 moved permanently 永久重定向
- - 302 found 临时重定向
- - 304 not modified 资源已找到，单位符合条件请求
- **4xx 客户端错误状态码 服务器无法处理请求**
- - 400 bad request 请求报文中有语法错误
- - 401 unauthorized 需要认证的请求
- - 403 forbidden 服务端拒绝请求
- - 404  not found
- **5xx 服务器错误状态码  服务器处理请求出错**
- - 500 internal server error 服务器执行请求时发生错误
- - 503 service unavaiable 超负载无法响应请求