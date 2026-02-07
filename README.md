## 前言

随着移动互联网的快速发展，校园订餐服务已成为大学生日常生活中不可或缺的一部分。本项目是基于微信小程序的校园订餐设计与开发，旨在为在校师生提供便捷、高效的订餐服务。

## 内容介绍

本项目主要包括以下功能模块：用户模块、商家模块、订单模块、菜品模块等。用户可以通过微信小程序查看附近商家及其菜品信息，完成在线点餐、支付、评论等操作。商家则可以通过后台管理系统进行菜品管理、订单处理、营业统计等操作。此外，本项目还具备以下特点：

1. 界面简洁，操作方便；
2. 支持多条件筛选，快速找到心仪的美食；
3. 实时查看订单状态，跟踪配送进度；
4. 严格的食品安全监管，保障用户权益。

## 技术介绍

本项目采用以下技术栈：

- 语言：Java
- 使用框架：Spring、Spring MVC、MyBatis、微信小程序
- 前端技术：JS、Vue、CSS3、Uniapp
- 开发工具：IDEA/Eclipse、Uniapp
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven：apache-maven 3.8.1-bin
- 前端环境：Node.js 12/14/16

## 核心代码

以下是项目中的一段核心代码，展示了如何实现用户登录功能：

```java
// 用户登录
@PostMapping("/login")
public Result login(@RequestBody User user) {
    // 查询用户信息
    User loginUser = userService.findByUsername(user.getUsername());
    if (loginUser != null && BCrypt.checkpw(user.getPassword(), loginUser.getPassword())) {
        // 登录成功，生成Token
        String token = jwtUtil.generateToken(loginUser);
        return Result.ok().data("token", token);
    } else {
        // 登录失败
        return Result.error().message("用户名或密码错误");
    }
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
![封面图片](https://img14.360buyimg.com/ddimg/jfs/t1/345538/12/3005/79736/68c5a626F51e9a99d/83c49b17aa613498.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/339379/32/10421/13027/68c5a5feF23e28f3c/dc318dccee7535fc.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/338042/34/10352/10137/68c5a5feF6961fb4d/d47387b6876041b8.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/342494/17/3058/11606/68c5a5ffF7fb052cb/7e9271d07d884ac4.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/351358/13/3122/37353/68c5a5ffFe7afdbf5/641c23e129ba6d9c.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/333126/34/12847/9232/68c5a600F05409db6/bbb29ad991273f26.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/326588/38/19841/30409/68c5a600Fee033afc/e02f902c56d19a29.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/350563/8/3047/33832/68c5a600F58298178/bf3052a9dc9fa875.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/323419/25/19909/60267/68c5a600F1f2ad5a7/1c42b46efecf330d.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/332296/37/12858/37777/68c5a601F236569fe/4d30601c2a5db28f.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
