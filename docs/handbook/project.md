# 1. demo示例

## 1.1后台代码创建

### 1.1.1 创建后台数据源

配置连接数据库信息，目前支持MySql、Oracle、SqlServer

注：只能连接系统部署的所在服务器能访问范围内的数据库。

选择自己所用的数据源类型，连接地址一般为项目数据库。

![创建数据源](..\images\addproject\创建数据源.png)

| 属性       | 描述                         | 必填 | 注意点     |
| ---------- | ---------------------------- | ---- | ---------- |
| 数据源名称 | 数据源的名称                 | 是   | 只用于标识 |
| 数据源类型 | MySql、Oracle、SqlServer     | 是   |            |
| 数据源驱动 | 连接各个数据库所使用的驱动包 | 是   |            |
| 连接地址   | 连接各个数据库的连接地址     | 是   |            |
| 用户名     | 数据库用户名                 | 是   |            |
| 密码       | 数据库密码                   | 是   |            |

### 1.1.2 数据库建表

数据库新建表，用于后端项目数据源(其属性设置按个人需求完善)，填写完毕保存并同步

![数据库建表](..\images\addproject\数据库建表.png)

| 属性   | 描述       | 必填 | 注意点 |
| ------ | ---------- | ---- | ------ |
| 表名   | 表名       | 是   |        |
| 表描述 | 对表的描述 | 是   |        |

对数据表的字段进行添加、修改、删除操作。

| 属性     | 描述       | 必填 | 注意点                 |
| -------- | ---------- | ---- | ---------------------- |
| 字段     | 字段名     | 是   | 根据各数据库的规则命名 |
| 类型     | 字段类型   | 是   |                        |
| 长度     | 字段长度   | 是   |                        |
| 比例     | 字段比例   | 否   |                        |
| 主键     | 是否是主键 | 否   |                        |
| 不是null | 是否不为空 | 否   |                        |
| 描述     | 字段描述   | 否   |                        |

【保存】：只是更改数据库

【保存并同步】：除了更改数据库，实体类和mapper映射也会同步更改

### 1.1.3 创建后端数据模型

数据模型是整个系统的核心，上面所有的功能都是为了数据模型的生成而准备的。通过数据表、模板和计划3方协助来完成。

选择自己所创建的数据源并给此次创建设置数据名称

![创建后端数据模型](..\images\addproject\创建后端数据模型.png)

| 属性   | 描述                                                         | 必填 | 注意点       |
| ------ | ------------------------------------------------------------ | ---- | ------------ |
| 类型   | 分为实体模型和非实体模型。实体模型是基于数据表、模板和计划生成，非实体模型只基于模板和计划生成 | 是   |              |
| 数据源 | 选择所添加的数据源                                           | 是   |              |
| 数据表 | 选择数据源下的数据表                                         | 是   |              |
| 编号   | 数据模型编号                                                 | 是   | 只能输入英文 |
| 名称   | 数据模型名称                                                 | 是   |              |
| 计划   | 生成数据模型所使用的计划                                     | 是   |              |

## 1.2设计前端页面

### 1.2.1创建前端数据模型

其中编号为菜单文件夹名称

![创建前端数据模型](..\images\addproject\创建前端数据模型.png)

| 属性 | 描述     | 必填 | 注意点       |
| ---- | -------- | ---- | ------------ |
| 编号 | 模块编号 | 是   | 只能输入英文 |
| 名称 | 模块名称 | 是   |              |

### 1.2.2创建前端页面

新建节点创建页面：

1.此处创建列表页、表单、流程表单

2.节点类型为对应页面类型，例：创建列表选择节点类型为列表

3.一般方便区分节点别名和文件名一样，模板使用默认列表模板(模板可在大厅主页按个人需求添加或编辑)，填写创建页面位置，创建完毕根据个人需求修改页面。

新建节点表：

| 属性     | 描述           | 值                                                 |
| -------- | -------------- | -------------------------------------------------- |
| 节点名称 | 节点的名称     |                                                    |
| 节点类型 | 节点的类型     | 表单/列表/其他                                     |
| 节点别名 | 节点的别名     |                                                    |
| 位置     | 文件创建的位置 | 相对位置   默认：src                               |
| 相对路径 | 相对路径       | 拼接在位置之后的路径  默认为数据模型编号，不可修改 |
| 文件名   | 文件名         |                                                    |
| 文件类型 | 文件类型       | 根据框架决定                                       |
| 模板     | 使用的模板文件 | 项目中可用的模板文件                               |

#### 1.2.2.1新建列表页面及设计内容

![新建节点](..\images\addproject\新建节点.png)
![新建节点二](..\images\addproject\新建节点二.png)

此处设计过程中列表中均绑定所需字段名称

![列表设计](..\images\project\列表设计.png)

#### 1.2.2.2新建表单页及设计内容

![表单](..\images\addproject\表单.png)
![表单设计](..\images\addproject\表单设计.png)

#### 1.2.2.3新建流程表单、设计流程表单内容

流程表单创建时模板选择流程表单

![流程表单](..\images\addproject\流程表单.png)
![流程表单设计](..\images\addproject\流程表单设计.png)

### 1.2.3创建前端接口

右击菜单页创建接口，选取后台项目中个人创建的数据模型自动生成接口信息，接口前缀：business。

![创建接口](..\images\addproject\创建接口.png)

| 属性     | 描述                         | 值                                                     |
| -------- | ---------------------------- | ------------------------------------------------------ |
| 选择模型 | 选择后台开发中创建的数据模型 |                                                        |
| 编号     |                              | 默认：选中数据模型的编号                               |
| 名称     | 接口文件名称                 |                                                        |
| 选择接口 | 选择需要创建的接口           | 默认：新增、修改、删除、详情查看（查单）、列表（查多） |
| 位置     | 文件创建路径                 | 默认：src                                              |
| 相对路径 | 拼接在位置属性之后的路径     | 默认：api                                              |
| 导入模块 | 需要导入的模块               | 默认：import request from ‘@/utils/request’            |

### 1.2.4添加前端项目页面菜单

根据前端设计器创建好列表和表单页面后，前端项目运行页面中添加列表页，在资源管理目录的基础模块引入列表页面，根据个人需求配置完善菜单添加内容，其中扩展属性：

路径：页面运行时浏览器地址栏路径

组件路径：页面跳转时所在项目中的相对路径，默认生成src/views/基础目录

![引入页面](..\images\project\添加页面.png)

刷新页面，打开对应添加的菜单位置，即可展示自己前台所建列表

![列表展示](..\images\project\列表展示.png)

## 1.3 功能实现

### 1.3.1引入创建的接口js

```
import {detail,delet,create,update,list,pageList} from '@/api/test_student'
```

![数据模型](..\images\project\引入api.png)

### 1.3.2修改请求列表方法，默认将getProjectList修改成接口js中的pageList

### 1.3.3 列表

#### 1.3.3.1添加和修改

列表通过路由打开表单，传入对应参数-表单类型、表单标题(按个人需求选择)、表单初始化数据

注：列表通过路由传入表单数据并接收时，表单赋值参数不要忘记新增对应全局变量，除表单已有变量，例：此处便于操作区分传入title，表单新增title全局变量，对应表单上方使用绑定title

添加事件，在method方法中添加add方法

```
 add() {
      // 跳转至页面
      this.$router.push({
        name: 'form',
        query: {
          type: "add",
          title:"添加",
          data:{}
        }
      });
    },
```

编辑事件，在编辑按钮中绑定edit事件传入行数据，然后在method方法中添加edit方法

```
  @click="edit(scope.row)"

```

```
 edit(row) {
      this.$router.push({
        name: "form",
        query: {
          type: "edit",
          title: "编辑",
          data: row,
        },
      });
    },
```

表单接受参数：执行代码写入方法中，方法将由mounted生命周期方法触发

```
    getData(){
      this.pageType = this.$route.query.type;
      this.title = this.$route.query.title;
      this.formData = this.$route.query.data
    }

```

填写表单数据或编辑表单数据并在表单内使用对应api传入对应所需参数,在method方法中写入保存事件方法

```
saveData() {
      if (this.pageType == "add") {
        create(this.formData).then((response) => {
          if (response.status == 1) {
            this.$message({
              type: "success",
              message: "保存成功",
            });
            this.closePage();
          }
        });
      } else {
        update(this.formData).then((response) => {
          if (response.status == 1) {
            this.$message({
              type: "success",
              message: "保存成功",
            });
            this.closePage();
          }
        });
      }
    },
```
![数据添加编辑](..\images\project\数据添加编辑.png)

#### 1.3.3.2删除

删除按钮绑定删除方法并传入行参数

```
  @click="del(scope.row)"

```
在列表页调用删除api写入删除方法传入所需行id

```
del(row) {
      this.$confirm("是否删除?", "提示", {
        confirmButtonText: "确定",
        cancelButtonText: "取消",
        type: "warning",
      })
        .then(() => {
          delet(row.id).then((result) => {
            if (result.status == 1) {
              this.getTableList();
              this.$message({
                type: "success",
                message: "删除成功!",
              });
            } else {
              this.$message({
                message: "删除失败!",
                type: "warning",
              });
            }
          });
        })
        .catch(() => {
          this.$message({
            type: "info",
            message: "已取消删除",
          });
        });
    },
```
![数据删除](..\images\project\数据删除.png)

#### 1.3.3.3查询

后台目录打开system-business/src/main/java/com.business/service/impl下的impl文件做出以下修改

![后台搜索逻辑](..\images\project\后台搜索逻辑.png)

搜索条件绑定字段keyword

![绑定字段](..\images\project\绑定搜索字段.png)

拷贝搜索字段并在列表数据请求方法中更换对应api

![更换列表api](..\images\project\更换列表api.png)

### 1.3.4表单
#### 1.3.4.1配置表单路由

![配置表单路由](..\images\project\配置表单路由.png)

#### 1.3.4.2表单引入api

![引入接口](..\images\project\引入api.png)

## 1.4设计流程页

点击流程进入流程设计
  
进入流程设计页显示登录， 初始账户：admin，初始密码：123456

![流程通道](..\images\project\流程通道.png)

### 1.4.1新建流程分类

新建流程分类用于模型创建时投入分类选择

![新建模型分类](..\images\project\新建模型分类.png)

### 1.4.2新建模型

点击设计进入设计页面

![流程设计按钮](..\images\project\流程设计按钮.png)
![新增模型](..\images\project\新增模型.png)

填写完毕点击确认进入设计页面

由开始节点启动，结束节点结束，中间插入任务板块，设计完成后保存模型并切换到模型管理界面

![节点说明](..\images\project\节点说明.png)

#### 1.4.2.1流程信息

1.流程信息：其中任务信息应用双引号包裹，表单url为流程表单路由path，具体配置参考菜单1.5.2

![流程信息](..\images\project\流程信息.png)

#### 1.4.2.2任务一

1.基础信息：任务名称设置位任务一

2.点击下方添加按钮添加处理命令

![任务一处理命令](..\images\project\任务一处理命令.png)

3.点击下方添加按钮添加任务分配并设置分配目标

![任务一任务分配](..\images\project\任务一任务分配.png)

#### 1.4.2.3任务二

1.基础信息：任务名称设置为任务二

2.处理命令：其中退回步骤表达式为：return "退回目标任务编号"(此处demo为退回任务一)

![任务二处理命令](..\images\project\任务二处理命令.png)

3.任务分配

![任务二任务分配](..\images\project\任务二任务分配.png)

设计完成点击保存

### 1.4.3导出模型

点击批量导出，再选择模型并下载模型到本地

![导出按钮](..\images\project\导出按钮.png)
![下载模型](..\images\project\下载模型.png)

## 1.5 流程表单

### 1.5.1流程模型导入发布

打开项目流程菜单，导入已经下载完毕的流程文件

![流程菜单打开](..\images\project\流程菜单打开.png)

解压本地已下载模型，上传对应文件，上传对应文件成功后点击发布

![流程模型导入](..\images\project\流程模型导入.png)

### 1.5.2流程表单修改

同表单类似，添加流程表单路由

![配置路由](..\images\project\配置路由.png)

#### 1.5.2.1引入api

![引入流程api](..\images\project\引入流程api.png)

#### 1.5.2.2表单绑定流程

添加标题字段(按个人需求添加)和新增formId字段

![新增字段](..\images\project\新增字段.png)

绑定主键id

![绑定主键](..\images\project\绑定主键.png)

businessKey：主键id

message:流程表单提交过程自动保存的一个信息参数字段，一般为意见审批流程的意见，此处绑定name不做参考可不绑定。

flowKey:模型流程key

![修改流程参数](..\images\project\修改流程参数.png)

#### 1.5.2.3接收路由参数

列表传入对应表单数据：表单页类型、表单标题(按个人需求)、表单id，由周期函数mounted触发接收路由参数getData()方法

```
  getData(){
    this.pageType = this.$route.query.type;
      this.title = this.$route.query.title;
      this.formId = this.$route.query.id;
  }

```

![触发接收参数方法](..\images\project\触发接收参数方法.png)

![接收路由参数](..\images\project\接收路由参数.png)

#### 1.5.2.4编写任务添加编辑逻辑

编写表单类型逻辑

```
if (!this.processConfig.isStart) {
      FlowProcess.comments().then((response) => {
        this.comments = response.data;
      });
      this.getById(this.processConfig.businessKey);
    }
    if(this.$route.query.type=="edit"){
          this.getById(this.formId);
     }
```

![判断流程进入类型和操作](..\images\project\判断流程进入类型和操作.png)

流程添加提交和更新流程信息逻辑方法修改

```
execute(event) {
      let target = event.currentTarget || event.target;
      if (this.processConfig.isStart) {
        if (this.$route.query.type == "add") {
          this.add(target);
        } else {
          this.update(target);
        }
      } else {
        this.update(target);
      }
    },
    getById(id) {
      detail(id).then((response) => {
        this.formData = response.data;
        this.processConfig.formData = this.formData;
      });
    },
    add(target) {
      this.formData.id = Date.now();
      create(this.formData).then((response) => {
        if (response.status == 1) {
          let commandevent = target.getAttribute("commandevent");
          this.commandEvent[commandevent]();
          this.dialogClose();
        }
      });
    },
    update(target) {
      update(this.formData).then((response) => {
        if (response.status == 1) {
          let commandevent = target.getAttribute("commandevent");
          this.commandEvent[commandevent]();
          this.dialogClose();
        }
      });
    },
```

![流程添加和编辑逻辑](..\images\project\流程添加和编辑逻辑.png)

### 1.5.3启动流程表单

点击添加按钮配置启动流程信息

注：启动前更改列表路由打开路径

![流程添加按钮](..\images\project\流程添加按钮.png)

流程启动：完善启动字段信息启动流程(确保流程主键不冲突，此处流程表单方法主键在方法中写入自动生成，也可将主键显示删除，不影响主键保存)

![提交启动一](..\images\project\提交启动一.png)

打开流程表单查看待办管理

![流程待办管理](..\images\project\流程待办管理.png)

结束流程，也可退回流程，填入意见信息，之后再操作完成，结束流程、

![结束流程](..\images\project\结束流程.png)

查看已办流程

![已办流程](..\images\project\已办流程.png)





















