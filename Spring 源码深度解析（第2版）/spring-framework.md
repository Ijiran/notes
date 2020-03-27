# 【一】整体架构 + 环境搭建

## spring整体架构

大约分为20个模块,书上大概列出了下面几种，模块一说，也只不过是针对spring有代表性的代码和功能进行总结而已，终究不能执着于死记硬背；根据具有代表性或者独立性的功能、具有特殊意义的代码来区分和记忆会更有效，也会对之后的开发起到性价比最高的作用。

### 1.Core Container （核心容器）

Core ： 基础模块，内含框架的一些基本的核心工具类，与其他包皆有关联。

Bean ： 基础模块，主要实现了访问配置文件、bean的创建和管理、IOC/DI操作等功能。

Context ： 在Core和Bean两个模块的基础之上构建，提供一种类似于JNDI注册器的框架的对象访问方法。

Expression Language ： 简称EL，提供了表达式语言，用于在运行时查询和操纵对象；也就是我们在jsp中常会使用的EL表达式。

### 2.Data Access/Integration

JDBC ： 提供了一个JDBC抽象层，封装了Spring对JDBC数据访问的类。

ORM ： 对象-关系映射模块。

OXM ： Object/XML映射模块。

JMS ： 消息服务模块。

Transaction ： 事务管理模块。

### 3.Web

Web ： 包括Web、Web-Servlet、Web-Struts、Web-Porlet等模块，使Spring充分支持Web开发。

### 4.AOP

AOP ： 提供面向切面编程的实现，使Spring集成AOP，使其无须依赖EJB组件。

### 5.Test

Test ： 集成JUnit、TestNG。

### 6.Aspects

Aspects： 提供了对AspectJ的集成支持。

### 7.Instrumentstion

Instrumentation ： 提供了class instrumentation  支持和classloader 实现。





# 【二】容器