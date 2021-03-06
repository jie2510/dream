# 2019.11.6
# Learning_plan  

## 一、学习Spring-boot框架  
### Level 1
1.配置好环境（Java开发环境，Spring-boot开发环境，MySQL环境）  
2.项目配置：创建一个练手项目，学会添加模块，配置项目。  
3.掌握三层代码结构编写DAO（Repository）、Servers、Controller，掌握组件的代码配置。  
4.学会测试。  
5.打包与部署：用maven命令打包发布与部署。  
6.循环练习，逐渐了解更多spring-boot细节，精益求精。 
### Level 2
1.学会更多IDEA功能（可选插件、快捷键等）  
2.系统梳理Spring-boot项目流程  
3.多练习运行几个demo，增加理解  
### Level 3  
1.逐渐往spring-boot原理（IOC，面向切面等）靠拢  
2.尝试自己搭建一个项目
 
## 二、学习知识图谱  
### Level 1
1.了解知识图谱相关内容及其在医疗领域的应用。  
2.尝试用python使用它。 
### Level 2
1.暂时还没想到，待打好spring-boot的基础和了解知识图谱基础知识后制定 

# 每日总结
- 2019.10.12
  - [x] 完成Idea安装与配置，通过IDEA上传项目到github上
- 2019.10.13
  - [x] 创建第一个HelloSpringboot项目，直观上感受了springboot程序运行过程；
  - [x] 复习了markdown语法继续熟悉IDEA的使用，发现它真的是一个很好的工具
  - [x] 发现一个[很适合初步感受Spring-boot流程的视频](https://www.bilibili.com/video/av39775932)
- 2019.10.14
  - [x] 成功安装mysql数据库，并在IDEA上配置好环境成功连接
  - [x] 熟悉了基本的mysql命令行，保留一份极简版本的[命令行大全](https://www.jianshu.com/p/14fc127f9663)以日后多多回顾
  - [x] 在测试IDEA连接mysql之余回顾了部分sql语句
  - [x] 继续练手HelloSpringboot项目，大概了解多url映射和参数传递
- 2019.10.15
  - [x] 进一步熟悉IDEA的基本功能
  - [x] 继续了解spring-boot的基本结构，解决了一个小疑惑[maven中的groupId和artifactId到底指的是什么？](https://blog.csdn.net/snowin1994/article/details/53024871)
- 2019.10.16
  - [x] [了解何为Servlet容器](https://blog.csdn.net/yw_1207/article/details/78706701)
  - [x] 为了更好地学习他人优秀的spring-boot项目，特意了解了一下前端框架Vue的基础
- 2019.10.17
  - [x] 大致了解了spring-boot体系中的Redis和Mybatis
  - [x] 由于对spring-boot的注解不太理解，找了一份相对来说不错的[spring-boot常用注解](https://blog.csdn.net/yitian_66/article/details/80866571)
- 2019.10.18
  - [x] 了解到了spring-boot的两种配置文件（properties文件和yml文件）的基础语法和基本用法。记录一下配置文件的作用是：修改springboot在底层为我们配置好了的默认值
  - [x] 自定义一个Person类，在yml文件配置其属性，然后在尝试在测试类中输出其toString()的值，但是失败了，test类中各种报错，尝试许久也无法解决，只能等到第二天再继续研究了
- 2019.10.19
  - [x] 解决了前一天遗留下来的无法运行test类的问题，原来spring-boot的自动导包技术有时会失灵，会通过maven导入一些不需要的jar包，而真正需要用到的包却不会自动下载。我的解决办法比较笨：删除项目中所有依赖的包，再通过Maven Reimport 
  - [x] 遇到一个无法注入bean的问题（明明代码是没有问题的呀.....）折腾许久终于明白Spring-boot自动扫描包成功与否与包路径的位置密切相关（注意存放自定义类的bean包与主程序类要在同一文件夹）具体看[关于SpringBoot bean无法注入的问题（与文件包位置有关）改变自动扫描的包](https://blog.csdn.net/u014695188/article/details/52263903)
  - [x] 了解到了更多配置文件的用法，尝试与理解Springboot自动配置文件的原理（懵懵懂懂的.....）
- 2019.10.20
  - [x] 了解了spring-boot的日志的大致功能(spirng-boot的日志采用的是slf4j+log4j配置方式)
  - [x] 尝试按网上教程模仿搭建一个简单的web项目，目前已了解了SpringBoot对静态资源的映射规则
- 2019.10.21
  - [x] 继续学习搭建web项目，目前已尝试使用了spring-boot的模板引擎thymeleaf，简单了解了thymeleaf的语法（感觉语法规则比较多，估计要花较多时间来熟悉）
  - [x] 简单学习了在spring-boot中使用Spring MVC的方法，但由于对Spring MVC还缺乏认识，目前进展不大
- 2019.10.23
  - [x] 尝试使用springboot模板引擎管理web网站的html页面，但是由于该练手项目需要配置的属性过多，暂时还未实现
  - [x] 了解了知识图谱的基础概念，本质上, 知识图谱旨在描述真实世界中存在的各种实体或概念及其关系,其构成一张巨大的语义网络图，节点表示实体或概念，边则由属性或关系构成。
- 2019.10.24
  - [x] 了解http请求报文头的内容，尝试通过模板引擎获取客户端请求报文的区域信息，然后实现页面语言切换操作
- 2019.10.25
  - [x] 成功通过jdbctemplate访问mysql数据库的数据表，将数据信息打印在一个html页面上
- 2019.10.26
  - [x] 成功研究使用jdbctemplate来连接数据库，实现对数据表的增删改查，但目前只是模仿别人的代码，对于原理等细节还不了解，接下来仍需继续研究，而且如何通过前端页面来操作数据库还有待学习。
- 2019.10.27
  - [x] 今天练习了使用springboot+Mybatis来连接mysql数据库，通过xml文档注入的形式实现了对数据的增删改查，在测试时学会用到postman工具
- 2019.11.6
  - [x] 了解了Sass模式的基本概念，Selenium测试框架的基本特点，尝试通过使用springboot+Mybatis注解的方式对数据的增删改查