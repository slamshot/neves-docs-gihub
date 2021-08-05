# 1. 环境配置、准备工作

## 1.1. 安装jdk

​需要 jdk1.8.0_171及以上

## 1.2. 安装数据库 

​支持 mysql，orcale，sqlserver数据库

## 1.3. redis、nacos、node

准备好redis、nacos、node 工具在下面下载服务插件安装后的文件目录env文件下有相关软件

注意：若使用平台设计器创建出来的前端项目，请使用提供的env文件下提供的版本的node环境

本项目中使

![工具](./images/install/工具.png)


# 2. 设计器服务安装与初始化必要数据

## 2.1. 服务安装

​双击Neves.exe文件进行安装

![安装界面](./images/install/server/1.png)

点击下一步选择安装路径

![安装1](./images/install/server/install1.png)

点击下一步安装

![安装2](./images/install/server/install2.png)

点击下一步然后完成安装

![安装3](./images/install/server/install3.png)

安装完成后的目录结构

![服务端目录](./images/install/服务端目录.png)

## 2.2. 初始化必要数据

​当安装成功后会弹出初始化界面

如果没有弹出请双击安装目录下的init.exe进行初始化操作

1. mySql和sqlServer数据无需手动创建数据库，可以直接初始化界面的数据库连接中填写数据库名称如下图

2. oracle数据库需要自己先创建用户，这里就不作用户创建的步骤了

3. 初始化数据库选项是对数据库初始化操作，如如果之前已经初始化过数据据，这里可不勾选

4. 用户和密码是你本地数据库的用户和密码    

![初始化](./images/install/server/初始化.png)



### 2.2.1 设计器配置

下面文件服务存储路径，文件服务地址，账号，密码是用户后面同步代码使用，这里可使用默认配置

对设计器配置进行初始配置，其中文件服务地址为内置minio，如需修改账号密码请到安装目录下的minio目录中参考minio官方文档进行修改

![安装程序](./images/install/server/5.png)  

填写完数据库信息 可以点击连接测试，测试成功点击下一步操作

![安装程序](./images/install/server/连接测试.png)  


### 2.2.2 流程配置

​ 对流程服务进行初始配置

![设计器配置](./images/install/server/6.png)

### 2.2.3 前台配置

​ 配置浏览器访问ip及端口

![设计器配置](./images/install/server/7.png)

## 2.3 启动服务

### 2.3.1 启动项目

初始化成功后​双击start.bat启动服务，等待项目启动，完成后将自动打开登录页面

​初始账号：admin  密码：123456

![登录页](./images/web/login.png)




# 3. 本地服务安装

## 3.1 下载服务插件

输入用户名密码后，登录进服务项目会提示下载服务插件，点击确定下载

![客户端提示](./images/install/server/客户端提示.png)

## 3.1 服务安装

​双击刚才下载的服务插件Neves.exe文件进行安装

![安装界面](./images/install/client/1.png)

点击下一步选择安装目录

![安装界面](./images/install/client/安装客户端1.png)

点下一步直接安装

![安装界面](./images/install/client/安装客户端2.png)

点击下一步完成安装

![安装界面](./images/install/client/安装客户端完成.png)

安装完成后的目录结构

![客户端目录](./images/install/客户端目录.png)


## 3.2 初始化必要数据

​​当安装成功后会弹出初始化界面

如果没有弹出请双击安装目录下的init.exe进行初始化操作

此时初始化加界面的信息中如果2.2初始化必要数据时没有修改ip端口，文件服务地址和秘密，这里使用默认即可

账号admin，密码123456

​![配置界面](./images/install/client/3.png)

填写信息 可以点击连接测试，测试成功点击下一步操作

![安装程序](./images/install/server/连接测试.png)  

## 3.3  启动服务

测试成功后

​双击安装目录下的nevesClient.bat启动服务，等待项目启动，完成后将自动打开登录页面

用户名admin  密码 123456
![登录页](./images/web/login.png)

# 4. 注意事项

如果切换了网络环境请重新初始化数据，重复2.2和3.2操作

重新初始化2.2操作不要勾选初始化数据选项

![重新初始化操作](./images/install/server/重新初始化操作.png)