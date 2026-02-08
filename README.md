## 前言

您好！这是一个基于微信小程序的点餐系统，采用SSM（Spring、SpringMVC、MyBatis）框架开发，前端使用JS、Vue、CSS3和Uniapp技术实现。本项目旨在为餐饮企业提供便捷的点餐服务，同时为开发者提供一个实践学习的案例。

## 内容介绍

本项目主要包括以下功能模块：用户模块、菜品模块、订单模块、后台管理模块。用户模块提供注册、登录、查看个人信息等功能；菜品模块负责展示菜品信息、分类和搜索；订单模块实现点餐、支付、订单查询等功能；后台管理模块包括菜品管理、订单管理、用户管理等功能。

## 技术介绍

- 语言：Java
- 使用框架：Spring、SpringMVC，MyBatis，微信小程序
- 前端技术：JS、Vue、CSS3，Uniapp
- 开发工具：IDEA/Eclipse，Uniapp
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven：apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是一段关于查询菜品的MyBatis核心代码：

```java
// Mapper接口
public interface DishMapper {
    @Select("SELECT * FROM dish WHERE id = #{id}")
    Dish selectDishById(@Param("id") Integer id);
}

// Service层
@Service
public class DishService {
    @Autowired
    private DishMapper dishMapper;

    public Dish getDishById(Integer id) {
        return dishMapper.selectDishById(id);
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
## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
