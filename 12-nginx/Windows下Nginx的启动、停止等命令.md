## **Windows下Nginx的启动、停止等命令**

在Windows下使用Nginx，我们需要掌握一些基本的操作命令，比如：启动、停止Nginx服务，重新载入Nginx等，下面我就进行一些简单的介绍。

假设你安装在 C:\server\nginx-1.0.2目录下，

cmd命令进入安装文件；

**1、启动：**

C:\server\nginx-1.0.2>start nginx

或

C:\server\nginx-1.0.2>nginx.exe

注：建议使用第一种，第二种会使你的cmd窗口一直处于执行中，不能进行其他命令操作。

**2、停止：**

C:\server\nginx-1.0.2>nginx.exe -s stop

或

C:\server\nginx-1.0.2>nginx.exe -s quit

注：stop是快速停止nginx，可能并不保存相关信息；quit是完整有序的停止nginx，并保存相关信息。

**3、重新载入Nginx：**

C:\server\nginx-1.0.2>nginx.exe -s reload

当配置信息修改，需要重新载入这些配置时使用此命令。

**4、重新打开日志文件：**

C:\server\nginx-1.0.2>nginx.exe -s reopen

**5、查看Nginx版本：**

C:\server\nginx-1.0.2>nginx -v