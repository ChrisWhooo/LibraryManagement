# LibraryManagement
基于jsp+servlet+mysql实现图书馆信息管理的javaweb小项目

开发工具：Eclipse

JDK:16.0

服务器：Tomcat9.0

数据库工具：mysql8.0+Workbench 8.0 CE

工作原理：浏览器和服务器通过http协议来建立连接，浏览器经过http的请求协议将用户想要的信息传到web服务器。之后，web服务器便会判断页面是静态还是动态。
如果是静态，web服务器会直接将用户想要的信息通过响应封装好之后再返回给浏览器；
如果是动态，web服务器会将接收到的内容传递给web容器，web容器再将内容传给servlet，（web容器在将信息传递给servlet的时候必须到web.xml的配置文件中去找到servlet的url-pattern路径），找到servlet后，web容器再启动一个servlet线程，然后再返回给web容器，web容器在将信息封装好传给web服务器，web服务器再将得到的信息解析后，通过响应封装，在传递到浏览器。

如下图所示：![微信图片_20230202143452](https://user-images.githubusercontent.com/101373296/216250148-475385ea-778e-4613-8f42-993571c50703.png)


#任务概述
该系统应能基本完成图书管理的基本要求。管理员可以对整个系统以及图书进行管理，用户可以进行借书还书等功能
1）	图书馆管理员可以查询全部图书的信息，可以对图书信息进行增删改
2）	图书管理员可以查询全部读者的信息，可以对读者信息进行增删改
3）	用户可以借书，还书和预约图书

系统用例图：

![image](https://user-images.githubusercontent.com/101373296/216250562-2f6370d4-247b-4cba-bf36-e4d1cc470dfd.png)
