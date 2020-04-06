**Tomcat体系结构**

Tomcat是⼀个Http服务器

Tomcat 设计了两个核⼼组件连接器（Connector）和容器（Container）来完成 Tomcat 的两⼤核⼼功能。

连接器：负责对外交流，处理Socket连接，负责网络字节流往Request和Response转换

容器组件：负责内部处理，加载和管理servlet，以及处理具体的request请求

![image-20200406212514253](C:\Users\yangyi\AppData\Roaming\Typora\typora-user-images\image-20200406212514253.png)

Catalina组件结构

Tomcat的核心组件，Tomcat就是一个Catalina实例

Catalina实例通过加载server.xml完成其他实例的创建，创建并管理⼀个Server，Server创建并管理多个服务，每个服务⼜可以有多个Connector和⼀个Container。

![image-20200406214332698](C:\Users\yangyi\AppData\Roaming\Typora\typora-user-images\image-20200406214332698.png)