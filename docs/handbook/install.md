# 一、安装

## 1.服务器端

### 1.1. 安装程序

​双击neves.exe![安装程序](./images/install/server/0.png)文件进行安装

​

![安装界面](./images/install/server/1.png)

​安装界面

​

### 1.2. 环境配置、准备工作

#### 1.2.1.  jdk

​需要 jdk1.8.0_171及以上

#### 1.2.2. 数据库 

​支持 mysql，orcale，sqlserver数据库

### 1.3. 初始化必要数据

​当安装成功后会弹出初始化界面/双击安装目录下的init.exe进行初始化操作



![安装程序](./images/install/server/5.png)

​初始化界面



#### 1.3.1 设计器配置

​  对设计器配置进行初始配置，其中文件服务地址为内置minio，如需修改账号密码请到安装目录下的minio目录中参考minio官方文档进行修改

​![设计器配置](./images/install/server/5.png)



#### 1.3.2 流程配置

​ 对流程服务进行初始配置

![设计器配置](./images/install/server/6.png)



#### 1.3.3 前台配置

​ 配置浏览器访问ip及端口

![设计器配置](./images/install/server/7.png)



### 1.4. 启动服务

​双击start.bat启动服务，等待项目启动，完成后将自动打开登录页面

​初始账号：admin  密码：123456

![登录页](./images/web/login.png)

​



## 2. 客户端

### 1.1. 安装程序

​双击winserver.exe ![登录页](./images/install/client/0.png)文件进行安装

​

![安装界面](./images/install/client/1.png)

​安装界面



### 1.2. 环境配置

#### 1.2.1.  jdk

​需要 jdk1.8.0_171及以上

### 1.3. 初始化必要数据

​当安装成功后会弹出初始化界面/双击安装目录下的init.exe进行初始化操作

​  

​![配置界面](./images/install/client/3.png)



### 1.4. 启动服务

​双击neves_winserver.exe启动服务，等待项目启动，完成后将自动打开登录页面

![登录页](./images/web/login.png)

