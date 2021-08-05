# 1. demo示例

## 1.1后台代码创建

### 1.1.1 创建后台数据源

![创建数据源](..\images\addproject\创建数据源.png)

### 1.1.2 数据库建表

数据库新建表，用于后端项目数据源，填写完毕保存并同步

![数据库建表](..\images\addproject\数据库建表.png)

### 1.1.3 创建后端数据模型

![创建后端数据模型](..\images\addproject\创建后端数据模型.png)

## 1.2设计前端页面

### 1.2.1创建前端数据模型

其中编号为菜单文件夹名称

![创建前端数据模型](..\images\addproject\创建前端数据模型.png)

### 1.2.2创建前端页面

新建节点创建页面，此处创建列表页、表单、流程表单，节点类型为列表，一般方便区分节点别名和文件名一样，模板使用列表模板，根据个人需求填写创建页面位置，创建完毕根据个人需求修改页面。

新建节点表：

| 属性     | 描述                                                  | 必填 | 注意点           |
| -------- | ----------------------------------------------------- | ---- | ---------------- |
| 节点类型 | model、example、dao、service、serviceImpl、controller | 是   | 只能输入英文     |
| 节点别名 | 用于编写模板时使用的别名                              | 是   | 只能输入英文     |
| 节点名称 | 用于在数据模型树展示的名称                            | 是   |                  |
| 位置     | 默认src/main/java                                     | 是   | 特殊情况可以修改 |
| 包名     | java文件的包名                                        | 是   |                  |
| 文件名   | java文件的文件名（类名）                              | 是   |                  |
| 文件类型 | java、xml（mybatis的映射文件）                        | 是   |                  |
| 类描述   | 类的描述                                              |      |                  |
| 模板     | 使用什么模板生成                                      | 是   |                  |
| 执行类   | 使用什么执行器生成代码                                | 是   | 可以自定义执行器 |

#### 1.2.2.1新建列表页面及设计内容

![新建节点](..\images\addproject\新建节点.png)
![新建节点二](..\images\addproject\新建节点二.png)
![列表设计](..\images\addproject\列表设计.png)

#### 1.2.2.2新建表单页及设计内容

![表单](..\images\addproject\表单.png)
![表单设计](..\images\addproject\表单设计.png)

#### 1.2.2.3新建流程表单、设计流程表单内容

![流程表单](..\images\addproject\流程表单.png)
![流程表单设计](..\images\addproject\流程表单设计.png)

### 1.2.3创建前端接口

右击菜单页创建接口，选取后台项目中个人创建的数据模型自动生成接口信息，接口前缀：business。

![创建接口](..\images\addproject\创建接口.png)

### 1.2.4添加前端项目页面菜单

根据前端设计器创建好列表和表单页面后，前端项目运行页面中添加列表页，在资源管理目录的基础模块引入列表页面，根据个人需求配置完善菜单添加内容，其中扩展属性：

路径：页面运行时浏览器地址栏路径

组件路径：页面跳转时所在项目中的相对路径，默认生成src/views/基础目录

![引入页面](..\images\project\添加页面.png)

打开对应添加的菜单位置，即可展示自己前台所建列表

![列表展示](..\images\project\列表展示.png)

## 1.3 功能实现

### 1.3.1引入创建的接口js

![数据模型](..\images\project\引入api.png)

### 1.3.2修改请求列表方法，默认将getProjectList修改成接口js中的pageList

### 1.3.3 列表

#### 1.3.3.1添加和修改

列表通过路由打开表单，传入对应参数-表单类型、表单标题(按个人需求选择)、表单初始化数据

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

编辑事件，在method方法中添加edit方法

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
      this.formId = this.$route.query.id;
      this.formData = this.$route.query.data
    }

```

填写表单数据或编辑表单数据并在表单内使用对应api,在method方法中写入保存事件方法

```
saveData() {
      if (this.pageType == "add") {
        create(this.formData).then((response) => {
          if (response.status == 1) {
            this.$message({
              type: "success",
              message: "保存成功",
            });
            this.$emit("refresh");
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
            this.$emit("refresh");
            this.closePage();
          }
        });
      }
    },
```

![数据添加编辑](..\images\project\数据添加编辑.png)

#### 1.3.3.2删除

调用删除api写入删除方法

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

列表中引入pageList搜索api

![引入搜索](..\images\project\引入搜索列表.png)

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

由开始节点启动，结束节点结束，中间插入任务板块，设计完成后保存模型并切换到模型管理界面

![节点说明](..\images\project\节点说明.png)

#### 1.4.2.1流程信息

1.流程信息：其中任务信息应用双引号包裹，表单url为流程表单路由path

![流程信息](..\images\project\流程信息.png)

#### 1.4.2.2任务一

1.基础信息：任务名称设置位任务一

2.处理命令

![任务一处理命令](..\images\project\任务一处理命令.png)

3.任务分配

![任务一任务分配](..\images\project\任务一任务分配.png)

#### 1.4.2.3任务二

1.基础信息：任务名称设置为任务二

2.处理命令：其中退回步骤表达式为：return "退回目标任务编号"(此处demo为退回任务一)

![任务二处理命令](..\images\project\任务二处理命令.png)

3.任务分配

![任务二任务分配](..\images\project\任务二处理命令.png)

### 1.4.3导出模型

点击批量导出，再选择模型并下载模型到本地

![导出按钮](..\images\project\导出按钮.png)
![下载模型](..\images\project\下载模型.png)

## 1.5 流程表单

### 1.5.1流程模型导入发布

解压本地已下载模型，上传对应文件，上传对应文件成功后点击发布

![流程模型导入](..\images\project\流程模型导入.png)

### 1.5.2流程表单修改

同表单类似，添加流程表单路由

![配置路由](..\images\project\配置路由.png)

#### 1.5.2.1引入流程api

![引入流程api](..\images\project\引入流程api.png)

#### 1.5.2.2表单绑定流程

添加标题字段(按个人需求添加)和新增formId字段

![新增字段](..\images\project\新增字段.png)

绑定主键id

![绑定主键](..\images\project\绑定主键.png)

businessKey：主键id

message:流程表单提交过程自动保存的一个信息参数字段，一般为意见审批流程的意见

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

流程添加提交和更新流程信息逻辑

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

![流程添加按钮](..\images\project\流程添加按钮.png)

流程启动：完善启动字段信息启动流程

![提交启动一](..\images\project\提交启动一.png)

打开流程表单查看待办管理

![流程待办管理](..\images\project\流程待办管理.png)

结束流程

![结束流程](..\images\project\结束流程.png)

查看已办流程

![已办流程](..\images\project\已办流程.png)





















