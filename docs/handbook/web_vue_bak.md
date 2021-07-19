###### 按钮

* 复制组件
* 删除组件
* 移动组件
![019设计页面](./images/019设计页面.png)
<br><br>

**类型**<br>
选择“表单”或“列表”类型，“表单”类型对应“属性页面”中“表单属性”，“列表”类型对应“属性页面”中“列表属性”
<br><br>

## 属性页面
***
“属性页面”用于调节“组件属性”、“表单属性”、“列表属性”
<br><br>

**窗口化**<br>
窗口化中的组件配置都对应的右侧配置
<br><br>

<h3>表单属性</h3><br>

***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>最外层元素</td>
<td>表单最外层元素标签</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">div/el-dialog/fawkes-dialog</td>
<td style="text-align: center;">el-dialog</td>
</tr>
<tr>
<td>表单标签</td>
<td>表单form的标签</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">el-form/fawkes-form</td>
<td style="text-align: center;">el-form</td>
</tr>
<tr>
<td>表单宽度</td>
<td>表单的宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">**px / **%</td>
<td style="text-align: center;">50%</td>
</tr>
<tr>
<td>标签对齐方式</td>
<td width="414">表单域标签的位置，如果值为 left 或者 right 时，<br />则需要设置&ldquo;表单字段宽度&rdquo;</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">右对齐/左对齐/顶部对齐</td>
<td style="text-align: center;">右对齐</td>
</tr>
<tr>
<td>表单字段标签宽度(px)</td>
<td width="414">表单域标签的宽度，例如 '50px'。<br />作为 Form 直接子元素的 form-item 会继承该值。支持 auto。</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>引入资源</td>
<td>页面需要引用的文件或组件.. 例：import { aa } from './api'</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>自定义样式</td>
<td>页面style标签内的内容</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>表单数据绑定</td>
<td>表单所有绑定数据的总对象</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">formData</td>
</tr>
<tr>
<td>表单验证</td>
<td>表单所有验证规则的总对象</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">formRules</td>
</tr>
<tr>
<td>自定义数据对象</td>
<td>data中定义的变量</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>组件尺寸</td>
<td>用于控制该表单内组件的尺寸</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">medium / small / mini</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>组件创建完成</td>
<td>在组件创建完成时触发</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>组件加载完成</td>
<td>在组件加载完成时触发</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>表单关闭</td>
<td>在页面关闭时触发</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--


**最外层元素**<br>
可选择最外层标签类型：div/el-dialog/fawkes-dialog(目前用于迪拜项目)
<br><br>

**表单标签**<br>
可选择表单form标签类型：el-form/fawkes-form(目前用于迪拜项目)
<br><br>

**表单宽度**<br>
表单的宽度，例如 '50%'
<br><br>

**标签对齐方式**
表单域标签的位置，如果值为"左对齐"或者"右对齐"时，则需要设置字段宽度
<br><br>

**表单字段宽度**<br>
表单域标签的字段宽度，例如 '50'
<br><br>

**引入资源**<br>
有页面需要引用的文件 例：import { aa } from './api'
<br><br>

**自定义样式**<br>
页面style标签内的内容
<br><br>

**表单绑定数据**<br>
* 表单数据绑定：用于表单的数据绑定
* 表单验证：用于表单的验证
<br><br>

**自定义数据对象**<br>
data中定义的变量
<br><br>

**组件尺寸**<br>
用于控制该表单内组件的尺寸,medium / small / mini
<br><br>

**事件**<br>
* 组件创建完成：在组件创建完成时触发
* 组件加载完成：在组件加载完成时触发
* 表单关闭：在表单关闭时触发
<br><br>

-->


<h3>列表属性</h3><br>

***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>宽度</td>
<td>页面宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>数据绑定对象</td>
<td>列表数据绑定的对象</td>
<td style="text-align: center;">array</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">listdata</td>
</tr>
<tr>
<td>引入资源</td>
<td>页面需要引用的文件或组件.. 例：import { aa } from './api'</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>自定义数据对象</td>
<td>data中定义的变量</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>自定义样式</td>
<td>页面style标签内的内容</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>组件创建完成</td>
<td>在组件创建完成时触发</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>组件加载完成</td>
<td>在组件加载完成时触发</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

**宽度**<br>
列表的宽度，例如 '50%'
<br><br>

**数据绑定**<br>
* 数据绑定对象：用于数据绑定对象
<br><br>

**自定义变量**<br>
用于data中自定义变量
<br><br>

**导入信息**<br>
导入信息用于需要引用的文件
<br><br>

**自定义样式**<br>
页面style标签内的内容
<br><br>


**事件**<br>
* 组件创建完成：在组件创建完成时触发
* 组件加载完成：在组件加载完成时触发
<br><br>

-->
<br><br>


# **布局组件**
## 表单Form
***
表单Form由文本框、按钮、单选框、多选框等控件组成，用以收集、校验、提交数据
<br><br>

**宽度**<br>
表单的宽度，例如 '50%'
<br><br>

**高度**<br>
表单的高度，例如 '200px'
![表单Form002](./images/表单Form002.png)
<br><br>

**数据绑定对象**<br>
“数据绑定字段”用于数据库字段（大小写一致）
<br><br>

**标签对齐方式**<br>
表单域标签的位置，如果值为"左对齐"或者"右对齐"时，则需要设置字段宽度，如图标签对齐方式为"左对齐"。
![表单Form003](./images/表单Form003.png)
<br><br>

**字段宽度**<br>
表单域标签的字段宽度，例如 '50'
![表单Form004](./images/表单Form004.png)
<br><br>

**组件尺寸**<br>
用于控制该表单内组件的尺寸,medium / small / mini
<br><br>

**自定义样式**<br>
用于表单style标签内的公共样式
<br><br>

## 栅格布局
***
通过基础的分栏，迅速简便地创建布局。
<br><br>

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>栅格间隔</td>
<td>栅格间隔</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">0</td>
</tr>
<tr>
<td>列配置项</td>
<td>配置每行列数及比例（一整行为24）</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>布局模式</td>
<td>布局模式，可选 flex，现代浏览器下有效</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>水平排列方式</td>
<td>flex 布局下的水平排列方式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">start/end/center/<br />space-around/space-between</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>垂直排列方式</td>
<td>flex 布局下的垂直排列方式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">top/middle/bottom</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

**栅格间距**<br>
分栏之间存在间隔,如图间隔距离为'10'
![栅格005](./images/栅格005.png)
<br><br>

**列配置项**<br>
通过基础的分栏任意添加删减列数以及列的大小形成布局。
![栅格006](./images/栅格006.png)
<br><br>

**布局模式**<br>
通过 flex 布局来对分栏进行灵活的对齐。
![栅格007](./images/栅格007.png)
<br><br>

**水平排列方式**<br>
flex 布局下的水平排列方式,可选'左对齐'、'右对齐'、'居中'、'两侧间隔相等'、'两段对齐'
<br><br>

**垂直排列方式**<br>
flex 布局下的垂直排列方式,可选'顶部对齐'、'居中'、'底部对齐'
<br><br>

-->

## 自定义布局
***
通过任意组件自定义组合设计形成需要的布局。
<br><br>

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>自定义元素标签</td>
<td>元素标签类型</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">div</td>
</tr>
<tr>
<td>元素框类型</td>
<td>布局元素 display 属性</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">block</td>
</tr>
<tr>
<td>宽度</td>
<td>布局宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>高度</td>
<td>布局高度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>自定义样式</td>
<td>改元素上的style属性</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>外边距</td>
<td>布局的外边距</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>内边距</td>
<td>布局的内边距</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>边框</td>
<td>布局的边框样式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>自定义属性</td>
<td>自由添加自定义的属性</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">&nbsp;</td>
</tr>
</tbody>
</table>

<!--
**自定义元素标签**<br>
可用于修改自定义布局元素标签类型
<br><br>

**元素框类型**<br>
布局元素 display 属性,可选类型'block'、'inline'、'inline-block'、'flex'、'list-item'、'table'、'inline-table'
<br><br>

**宽度、高度**<br>
用于设置自定义布局组件的宽度、高度，如'300px'
![自定义008](./images/自定义008.png)
<br><br>

**自定义样式**<br>
用于布局的style属性值
<br><br>

**外边距**<br>
用于设置自定义布局组件的外边距，可设置'上外边距'、'下外边距'、'左外边距'、'右外边距'，如'30px'
<br><br>

**内边距**<br>
用于设置自定义布局组件的内边距，可设置'上内边距'、'下内边距'、'左内边距'、'右内边距'，如'30px'
<br><br>

**边框**<br>
用于设置自定义布局组件上、下、左、右边框的宽度如'1px'，线条可选'实线'、'双实线'、'虚线'、'虚点'，颜色可随意选择。
<br><br>

**自定义属性**<br>
用于添加自定义的属性及属性值
<br><br>

-->
<br><br>

## 列表/明细表
***

<table width="1359">
<tbody>
<tr style="text-align: center;">
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td style="text-align: left;" colspan="5">列属性</td>
</tr>
<tr>
<td>绑定字段</td>
<td>对应列内容的字段名</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>名称</td>
<td>显示的标题</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>宽度</td>
<td>对应列的宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>对齐方式</td>
<td>对应列内容的对齐方式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">left/center/right</td>
<td style="text-align: center;">center</td>
</tr>
<tr>
<td>内容过长隐藏</td>
<td>当内容过长被隐藏时显示 tooltip</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>是否排序</td>
<td width="414">对应列是否可以排序，如果设置为 'custom'，<br />则代表用户希望远程排序，需要监听 Table 的 sort-change 事件</td>
<td style="text-align: center;">boolean, string</td>
<td style="text-align: center;">true, false, 'custom'</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>格式化</td>
<td>用来格式化内容</td>
<td style="text-align: center;" width="301">Function(row, column<br />, cellValue, index)</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="text-align: left;" colspan="5">工具栏配置</td>
</tr>
<tr>
<td>是否显示</td>
<td>控制工具栏是否显示</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">TRUE</td>
</tr>
<tr>
<td>文字</td>
<td>列表名称</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>按钮整体样式</td>
<td>设置工具栏整体样式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>按钮配置</td>
<td>配置工具栏按钮&nbsp; 按钮配置详见按钮组件</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td style="text-align: left;" colspan="5">基础配置</td>
</tr>
<tr>
<td>数据绑定对象</td>
<td>列表数据绑定的对象</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>数据选中对象</td>
<td>列表选中数据集合</td>
<td style="text-align: center;">array</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否生成el-form及el-form-item标签</td>
<td>控制其中组件是否生成el-form-item标签</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>表头对齐方式</td>
<td>表头对齐方式，若不设置该项，则使用表格的对齐方式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">left/center/right</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>表头样式</td>
<td>表头行样式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>组件类型</td>
<td>列表与明细表之间切换</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>选择模式</td>
<td>列表的选择模式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">多选/单选</td>
<td style="text-align: center;">多选</td>
</tr>
<tr>
<td>列表高度</td>
<td>列表的高度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>表格尺寸</td>
<td>列表table的尺寸</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>组件尺寸</td>
<td>列表/明细表中的组件大小</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否显示序号列</td>
<td>列表是否显示序号</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">TRUE</td>
</tr>
<tr>
<td>加载文本</td>
<td>加载时显示文字</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td style="text-align: left;" colspan="4">分页栏配置</td>
<td>&nbsp;</td>
</tr>
<tr>
<td>是否显示分页</td>
<td>控制分页栏是否显示</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>分页栏位置</td>
<td>控制分页栏位置</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">left center right</td>
<td style="text-align: center;">left</td>
</tr>
<tr>
<td>每页条数</td>
<td>列表每页数据量</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">15</td>
</tr>
<tr>
<td width="262">是否为分页按钮添加背景色</td>
<td>是否为分页按钮添加背景色</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>分页子组件</td>
<td>组件布局，子组件名用逗号分隔</td>
<td style="text-align: center;">String</td>
<td style="text-align: center;" width="229">sizes,&nbsp;prev,&nbsp;pager,&nbsp;next,<br />&nbsp;jumper,&nbsp;-&gt;,&nbsp;total,&nbsp;slot</td>
<td style="text-align: center;" width="153">prev, pager, next, jumper, -&gt;, total'</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>排序事件</td>
<td>当表格的排序条件发生变化的时候会触发该事件</td>
<td>function({ column, prop, order })</td>
</tr>
<tr>
<td>当前选中行改变时</td>
<td>当用户手动勾选数据行的 Checkbox 时触发的事件</td>
<td>function(selection, row)</td>
</tr>
<tr>
<td>选中行改变事件</td>
<td>当选择项发生变化时会触发该事件</td>
<td>function(selection)</td>
</tr>
<tr>
<td>全选事件</td>
<td>当用户手动勾选全选 Checkbox 时触发的事件</td>
<td>function(selection)</td>
</tr>
<tr>
<td>取消全选事件</td>
<td>取消全选时触发</td>
<td>&mdash;</td>
</tr>
<tr>
<td>分页大小改变事件</td>
<td>pageSize 改变时会触发</td>
<td>function(pageSize)</td>
</tr>
<tr>
<td>页码改变事件</td>
<td>currentPage 改变时会触发</td>
<td>function(currentPage)</td>
</tr>
</tbody>
</table>

<!--
**列配置**<br>
用于配置列的属性，点击“配置”按钮，进入到列配置界面
![列表009](./images/列表009.png)
* 绑定字段：用于数据库绑定字段（大小写一致）
* 名称：用于设置此列表头名称
* 宽度：用于设置此列宽度，如'30px'
* 对齐方式：用于设置此列数据对齐方式，可选'左对齐'、'居中'、'右对齐'
* 过长隐藏提示：选择内容过长时是否隐藏并提示
* 是否排序：对应列是否可以排序
* 格式化：用来格式化内容
* 操作：用于添加删除列以及对列进行上移、下移的调整
* 添加：用于添加列
* 重置：用于重置设置的属性
<br><br>

**工具栏配置**<br>
* 是否显示：用于选择是否显示工具栏
* 文字：用于设置工具栏的文字
* 工具栏按钮整体样式：用于设置工具栏按钮整体样式
* 按钮配置：用于配置按钮属性，点击“按钮配置”按钮，进入按钮配置界面<br>
![列表010](./images/列表010.png)
* 文字：用于设置按钮的文字
* 文字位置：用于设置按钮文字在'图标前'或'图标后'
* 图标：用于设置图标样式
* 风格：用于设置按钮风格，可选'默认'、'朴素'、'圆形'
* 类型：用于设置按钮类型，可选'文本按钮'、'主要按钮'、'成功按钮'、'信息按钮'、'警告按钮'、'危险按钮'
* 事件：按钮点击时触发的事
* 操作：用于添加删除按钮以及按钮进行上移、下移的调整
* 重置：用于重置设置的属性

**基础配置**<br>
* 数据绑定对象：明细表/列表绑定的数据对象名称
* 数据选中对象：用以存储选中数据的对象名称
* 是否生成el-form及el-form-item标签：组件是否生成el-form及el-form-item标签
* 表头对齐方式：用于设置表头列名称的对齐方式，可选'left'、'center'、'right'
* 表头样式：用于设置表头的样式
* 组件类型：用于选择组件的类型'列表'或'明细表'，选择不同的类型，对应有特有的属性
* 选择模式<label style="color:red">（列表特有属性）</label>：数据选择模式“单选”或者“多选”
* 列表高度：可选“自适应”或“固定”，选择“自适应”，设置去除高度，如'50px'，选择“固定”，设置固定高度，如'50px'
* 表格尺寸：可选表格的尺寸，“大”、“中”、“小”三种尺寸
* 组件尺寸<label style="color:red">（列表特有属性）</label>：可选组件的尺寸，“大”、“中”、“小”三种尺寸
* 自定义加载文本<label style="color:red">（列表特有属性）</label>：自定义设置加载的文本内容
* 是否显示序列号<label style="color:red">（列表特有属性）</label>：是否显示列表序号
<br><br>

**分页栏**<label style="color:red">（列表特有属性）</label><br>
* 是否显示分页：是否显示列表分页
![列表016](./images/列表016.png)
* 分页栏位置：可选分页栏位置，'left'、'center'、'right'，如'center'
![列表017](./images/列表017.png)
* 每页条数：可设置分页栏每页条数，如'15'
* 是否为分页按钮添加背景色：可选是否为分页栏按钮添加背景色
![列表018](./images/列表018.png)
* 分页子组件：用于设置分页栏的子组件
<br><br>

**事件**<br>
* 排序事件：在排序时触发
* 当前选中行改变时：在当前选中行改变时触发
* 选中行改变事件：在选中行改变时触发
* 全选事件：在全选时触发
* 取消全选事件：在取消全选时触发
* 分页大小改变事件：在分页大小改变时触发
* 页码改变事件：在页码改变时触发
<br><br>

-->

# **基础组件**
## **基础属性**
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>表单item标签</td>
<td>可选择组件外层form-item标签的类型</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">el-form-item<br />fawkes-form-item</td>
<td style="text-align: center;">el-form-item</td>
</tr>
<tr>
<td>标题</td>
<td>标签文本&nbsp;&nbsp; 变量：是否为变量</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>宽度</td>
<td>调节组件的宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>id</td>
<td>组件元素标签id</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>自定义class</td>
<td>组件class属性</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>显示条件</td>
<td>组件显示的条件</td>
<td style="text-align: center;">function</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>数据绑定字段</td>
<td>绑定的数据对象</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>默认值</td>
<td>组件默认值</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br>

组件其他配置:包含组件的不常有用配置项，也可自定义添加属性
<!--
**表单item标签**<br>
可选择组件外层form-item标签的类型，已有类型：el-form-item以及fawkes-form-item(目前用于迪拜项目)
<br><br>

**标题**<br>
* 变量：填写变量的选项
* 用于输入框前的标题名称，如“姓名”
<br><br>

**宽度**<br>
用于调节“文本框”组件的大小，如'50%'
<br><br>

**id**<br>
用于输入页面标签元素的id
<br><br>

**自定义class**<br>
用于输入需要额外增加的class模式，class的名称例如：form sp
<br><br>

**显示条件**<br>
组件显示的条件  返回true（显示）/false (不显示)
<br><br>

**数据绑定字段**<br>
用于数据库字段（大小写一致）
<br><br>

-->

## 文本框
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td colspan="4">常用配置</td>
<td>&nbsp;</td>
</tr>
<tr>
<td>占位内容</td>
<td>输入框占位文本</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>禁用</td>
<td>禁用</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>显示清除按钮</td>
<td>是否可清空</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>必填</td>
<td>是否为必填&nbsp; 可选择类型及配置提示文字及触发时机</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>值改变事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>失去焦点事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>获得焦点事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>清空按钮点击事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--
<h3>基础配置</h3><br>

**默认值**<br>
输入框内默认的值
* 静态：字符串
* 动态：可以写方法调用获取
<br><br>

**常用配置**<br>
**占位内容**<br>
输入框占位文本（灰底文字），如“占位”
![文本框012](./images/文本框012.png)
<br><br>

**操作属性**
* 禁用：组件是否禁用
* 显示清除按钮：输入框文本是否可清空
<br><br>

**校验**<br>
* 必填：输入框是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
* 类型：输入框填写的文本类型，可选“数字”、“整数”、“浮点数”、“URL地址”、“邮箱地址”
<br><br>

**事件**<br>
* 值改变事件：在 Input 值改变时触发
* 失去焦点事件：在 Input 失去焦点时触发
* 获得焦点事件：在 Input 获得焦点时触发
* 清空按钮点击事件：在点击由 clearable 属性生成的清空按钮时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值

-->

## 文本
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>文字</td>
<td>span的内容</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>高度</td>
<td>span的高度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>行高</td>
<td>span的行高</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>字号</td>
<td>文字大小</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>颜色</td>
<td>文字颜色</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

<h3>基础配置</h3><br>

**文字**<br>
输入文字，如“文字”
<br><br>

**高度**<br>
用于调节“文本”组件的大小，如'300px'
<br><br>

**行高**<br>
line-height，如'60px'
<br><br>

**字号**<br>
用于调节文本字体大小，如'20px'
<br><br>

**颜色**<br>
可选择文字字体的颜色
<br><br>

-->

## 文本域
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>最小行数</td>
<td>文本域最小的行数,同时设置最大行数时固定行数将失效</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>最大行数</td>
<td>文本域最大的行数,同时设置最小行数时固定行数将失效</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>固定行数</td>
<td>文本域固定的行数</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>最大输入长度</td>
<td>文本域内最大输入的字符数量</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>占位内容</td>
<td>输入框占位文本</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否显示输入字数统计</td>
<td>是否显示输入字数统计</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>必填</td>
<td>是否为必填&nbsp; 可选择类型及配置提示文字及触发时机</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">FALSE</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>值改变事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">function(value)</td>
</tr>
<tr>
<td>失去焦点事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>获得焦点事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>清空按钮点击事件</td>
<td>&nbsp;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

<h3>基础配置</h3><br>

**默认值**<br>
输入框内默认的值
* 静态：字符串
* 动态：可以写方法调用获取
<br><br>

<h3>常用配置</h3><br>

**最小行数**<br>
用于设置文本域最小的行数,如'1'
<br><br>

**最大行数**<br>
用于设置文本域最大的行数，如'10'
<br><br>

**固定行数**<br>
用于设置文本域固定的行数，如'5'
<br><br>

**最大输入长度**<br>
用于设置文本域内最大输入的字符数量，如'10'
<br><br>

**占位内容**<br>
输入框占位文本（灰底文字），如“占位”
<br><br>

**操作属性**
* 禁用：组件是否禁用
* 显示输入字数统计：是否显示输入字数统计
<br><br>

**校验**<br>
* 必填：输入框是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**事件**<br>
* 值改变事件：在 Input 值改变时触发
* 失去焦点事件：在 Input 失去焦点时触发
* 获得焦点事件：在 Input 获得焦点时触发
* 清空按钮点击事件：在点击由 clearable 属性生成的清空按钮时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值

-->


## 计数器
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>最小值</td>
<td>最小值</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>最大值</td>
<td>最大值</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>步长</td>
<td>步长</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">1</td>
</tr>
<tr>
<td>禁用</td>
<td>禁用</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**最小值**<br>
用于设置计数器最小的值，如'1'
<br><br>

**最大值**<br>
用于设置计数器最大的值,如'100'
<br><br>

**步长**<br>
设置递增递减的步数，如'5'
<br><br>

**操作属性**
* 禁用：组件是否禁用
<br><br>

**校验**<br>
* 必填：计数器是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->


## 单选组
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td width="153">默认值</td>
</tr>
<tr>
<td>布局方式</td>
<td>选项布局方式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">行内/块级</td>
<td style="text-align: center;">行内</td>
</tr>
<tr>
<td>静态数据</td>
<td>固定数据</td>
<td style="text-align: center;">array</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>动态数据</td>
<td>动态获取数据方法</td>
<td style="text-align: center;">function</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>禁用</td>
<td>禁用</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>必填</td>
<td>是否为必填&nbsp; 可选择类型及配置提示文字及触发时机</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>值改变</td>
<td>选中值改变时触发</td>
<td style="text-align: center;">function(value)</td>
</tr>
</tbody>
</table>

<!--
<h3>常用配置</h3><br>

**布局方式**<br>
用于设置单选组选项的布局方式，可选“块级”或“行内”
<br><br>

**静态数据**<br>
用于添加选项
* 实际值：存入数据库的值
* 显示值：显示的值
* 禁用：是否可选
<br><br>

**动态数据**<br>
添加调用的方法来获取数据
<br><br>

**操作属性**
* 禁用：组件是否禁用
<br><br>

**校验**<br>
* 必填：计数器是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**事件**<br>
* 值改变事件：在 Input 值改变时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->

## 多选组
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td width="153">默认值</td>
</tr>
<tr>
<td>布局方式</td>
<td>选项布局方式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">行内/块级</td>
<td style="text-align: center;">行内</td>
</tr>
<tr>
<td>静态数据</td>
<td>固定数据</td>
<td style="text-align: center;">array</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>动态数据</td>
<td>动态获取数据方法</td>
<td style="text-align: center;">function</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>禁用</td>
<td>禁用</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>必填</td>
<td>是否为必填&nbsp; 可选择类型及配置提示文字及触发时机</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>值改变</td>
<td>选中值改变时触发</td>
<td style="text-align: center;">function(value)</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**布局方式**<br>
用于设置多选组选项的布局方式，可选“块级”或“行内”
<br><br>

**静态数据**<br>
用于添加选项
* 实际值：存入数据库的值
* 显示值：显示的值
* 禁用：是否可选
<br><br>

**动态数据**<br>
添加调用的方法来获取数据
<br><br>

**操作属性**
* 禁用：组件是否禁用
<br><br>

**校验**<br>
* 必填：计数器是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**事件**<br>
* 值改变事件：在 Input 值改变时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->

## 日期
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>最小值</td>
<td>可选日期的最小值</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>最大值</td>
<td>可选日期的最大值</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>显示类型</td>
<td>选择日期的显示类型</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">如'year'、'month'、'date'、<br />'dates'、 'datetime'、<br />'datetimerange'、' daterange'</td>
<td style="text-align: center;">date</td>
</tr>
<tr>
<td>占位内容</td>
<td>输入框占位文本</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>格式</td>
<td>日期格式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>选择框对齐方式</td>
<td>对齐方式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>默认值</td>
<td>默认值</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**最小值**<br>
用于设置日期最小值，如'2019-11-01'
<br><br>

**最大值**<br>
用于设置日期最大值，如'2019-12-31'
<br><br>

**显示类型**<br>
选择日期的显示类型，如'year'、'month'、'date'、'dates'、 'datetime'、'datetimerange'、' daterange'
<br><br>

**占位内容**<br>
输入框占位文本（灰底文字），如“占位”
<br><br>

**格式**<br>
可选日期显示的格式，如“yyyy年MM月”
![日期014](./images/日期014.png)
<br><br>

**选择框对齐方式**<br>
可选日期选择框的对齐方式，如'left'
![日期015](./images/日期015.png)
<br><br>

**默认值**<br>
用于设置默认的日期值
<br><br>

**操作属性**
* 禁用：组件是否禁用
* 文本框可输入：文本框是否可输入
* 显示清除按钮：文本框是否可清空
<br><br>

**校验**<br>
* 必填：输入框是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**事件**<br>
* 值改变事件：在 Input 值改变时触发
* 失去焦点事件：在 Input 失去焦点时触发
* 获得焦点事件：在 Input 获得焦点时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->


## 下拉选择框
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>占位内容</td>
<td>输入框占位文本</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">&nbsp;</td>
</tr>
<tr>
<td>是否多选</td>
<td>是否多选</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>选中值按文字的形式展示</td>
<td>多选时是否将选中值按文字的形式展示</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>静态数据</td>
<td>固定数据</td>
<td style="text-align: center;">array</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>动态数据</td>
<td>动态获取数据方法</td>
<td style="text-align: center;">function</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>搜索配置</td>
<td>配置无匹配时显示文字及选项为空时显示</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>必填</td>
<td>是否为必填&nbsp; 可选择类型及配置提示文字及触发时机</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>值改变</td>
<td>选中值改变时触发</td>
<td style="text-align: center;">目前的选中值</td>
</tr>
<tr>
<td>清空</td>
<td>可清空的单选模式下用户点击清空按钮时触发</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>失去焦点</td>
<td>当 input 失去焦点时触发</td>
<td style="text-align: center;">(event: Event)</td>
</tr>
<tr>
<td>获得焦点</td>
<td>当 input 获得焦点时触发</td>
<td style="text-align: center;">(event: Event)</td>
</tr>
<tr>
<td>下拉框出现/隐藏</td>
<td>下拉框出现/隐藏时触发</td>
<td style="text-align: center;">出现则为 true，隐藏则为 false</td>
</tr>
<tr>
<td>移除tag(多选)</td>
<td>多选模式下移除tag时触发</td>
<td style="text-align: center;">移除的tag值</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**占位内容**<br>
输入框占位文本（灰底文字），如“占位”
<br><br>

**操作属性**<br>
* 是否多选：选择是否多选
* 选中值按文字的形式展示：是否按文字的形式展示选中的选项
<br><br>

**静态数据**<br>
用于添加选项
* 实际值：存入数据库的值
* 显示值：显示的值
<br><br>

**动态数据**<br>
添加调用的方法来获取数据
<br><br>

**搜索配置**<br>
* 无匹配显示：搜索时无结果显示文字
* 选项为空时显示：下拉选选项为空时显示文字
<br><br>

**校验**<br>
* 必填：输入框是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**事件**<br>
* 值改变：在值改变时触发
* 清空：在清空时触发
* 失去焦点：在失去焦点时触发
* 获得焦点：在获得焦点时触发
* 下拉框出现/隐藏：在下拉框出现/隐藏时触发
* 移除tag（多选）：在移除tag(多选)时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->

## 结构树
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>高亮当前节点</td>
<td>是否高亮当前选中节点，默认值是 false。</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>展开所有节点</td>
<td>是否默认展开所有节点</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>单节点展开</td>
<td>是否每次只打开一个同级树节点展开</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>节点是否可选</td>
<td>节点是否可被选择</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>数据方法</td>
<td>获取数据的方法</td>
<td style="text-align: center;">function</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">&nbsp;</td>
</tr>
<tr>
<td>父字段</td>
<td>指定节点标签为节点对象的某个属性值</td>
<td style="text-align: center;">string, function(data, node)</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>子字段</td>
<td>指定子树为节点对象的某个属性值</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**操作属性**<br>
* 高亮当前节点：是否高亮当前节点
* 展开所有节点：是否展开所有节点
* 单节点展开：是否单节点展开
* 节点是否可选：节点是否可以选择
<br><br>

**数据**<br>
* 方法：获取结构树数据的方法
* 父字段：指定节点标签为节点对象的某个属性值
* 子字段：定子树为节点对象的某个属性值
<br><br>

-->

## 文件上传
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>上传地址</td>
<td>上传的地址</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>最大上传数</td>
<td>最大允许上传个数</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>文件类型</td>
<td>接受上传的文件类型（thumbnail-mode 模式下此参数无效）</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>上传的文件字段名</td>
<td>上传的文件字段名</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">file</td>
</tr>
<tr>
<td>额外参数</td>
<td>上传时附带的额外参数</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>按钮文字</td>
<td>按钮文字内容</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>提示文字</td>
<td>按钮下方提示文字</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>禁用&nbsp;</td>
<td>禁用&nbsp;</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>多文件上传</td>
<td>是否支持多选文件</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否自动上传</td>
<td>是否在选取文件后立即进行上传</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否显示文件列表</td>
<td>是否显示已上传文件列表</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>上传前</td>
<td width="414">上传文件之前的钩子，参数为上传的文件，<br />若返回 false 或者返回 Promise 且被 reject，则停止上传。</td>
<td style="text-align: center;">function(file)</td>
</tr>
<tr>
<td>上传成功</td>
<td>文件上传成功时的钩子</td>
<td style="text-align: center;">function(response, file, fileList)</td>
</tr>
<tr>
<td>上传失败</td>
<td>文件上传失败时的钩子</td>
<td style="text-align: center;">function(err, file, fileList)</td>
</tr>
<tr>
<td>预览</td>
<td>点击文件列表中已上传的文件时的钩子</td>
<td style="text-align: center;">function(file)</td>
</tr>
<tr>
<td>删除时</td>
<td>文件列表移除文件时的钩子</td>
<td style="text-align: center;">function(file, fileList)</td>
</tr>
<tr>
<td>删除前</td>
<td width="414">删除文件之前的钩子，参数为上传的文件和文件列表，<br />若返回 false 或者返回 Promise 且被 reject，则停止删除。</td>
<td style="text-align: center;">function(file, fileList)</td>
</tr>
<tr>
<td>超出限制</td>
<td>文件超出个数限制时的钩子</td>
<td style="text-align: center;">function(files, fileList)</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**上传地址**<br>
需要调用的上传接口名称
<br><br>

**最大上传数**<br>
限制文件最大上传数量，如'3'
<br><br>

**文件类型**<br>
文件的后缀名，多种类型以逗号分隔，如'.jpg'，'.doc'
<br><br>

**上传的文件字段名**<br>
后台接口中接收文件的参数名称
<br><br>

**额外参数**<br>
上传时附带的额外参数
<br><br>

**按钮文字**<br>
文件上传时点击的按钮的名称，如“选择文件”
<br><br>

**提示文字**<br>
文件上传时的提示，如“请上传XXX文件”
<br><br>

**操作属性**<br>
* 禁用：组件是否禁用
* 多文件上传：是否多文件上传
* 是否自动上传：是否自动上传文件
* 是否显示文件列表：是否显示上传的文件
<br><br>

**事件**<br>
* 上传前：在上传前触发的事件
* 上传成功：在上传成功时触发的事件
* 上传失败：在上传失败时触发的事件
* 预览：在预览时触发的事件
* 删除时：在删除时触发的事件
* 删除前：在删除前触发的事件
* 超出限制：在超出限制时触发的事件
<br><br>

-->

## 按钮
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>文字位置</td>
<td>有图标时文字所处位置</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">前/后</td>
<td style="text-align: center;">后</td>
</tr>
<tr>
<td>文字</td>
<td>按钮文字</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>按钮图标</td>
<td>按钮图标</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>按钮风格</td>
<td>按钮风格</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">朴素按钮&nbsp;圆形按钮</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>按钮类型</td>
<td>按钮类型</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">文本按钮&nbsp;主要按钮&nbsp;成功按钮<br />&nbsp;信息按钮&nbsp;警告按钮&nbsp;危险按钮</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>禁用</td>
<td>禁用</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>点击事件</td>
<td>点击事件</td>
<td style="text-align: center;">function</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<!--
<h3>基础配置</h3><br>

**文字位置**<br>
可选文字位置在“图标前”或“图标后”，如选“图标前”的预览效果
![按钮016](./images/按钮016.png)
<br><br>

**文字**<br>
按钮的文字，如“确定”
<br><br>

**按钮图标**<br>
目前只能填写https://element.eleme.cn/2.0/#/zh-CN/component/icon 该地址上的按钮图标名称，如' el-icon-warning'
<br><br>

**按钮风格**<br>
可选按钮的风格，“朴素按钮”或“圆形按钮”
<br><br>

**按钮类型**<br>
可选按钮的类型，“文本按钮”、“主要按钮”、“成功按钮”、“信息按钮”、“警告按钮”、“危险按钮”
<br><br>

**操作属性**
* 禁用：组件是否禁用
<br><br>

**事件**
* 点击事件：在点击时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->

# **第三方组件**
## ecidi列表
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>标签宽度</td>
<td>搜索栏组件标签宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>当前页绑定对象</td>
<td>当前页变量</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>每页数据量绑定对象</td>
<td>每页数变量</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>数据总数绑定对象</td>
<td>列表数据总数变量</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>列表名称</td>
<td>列表的名称</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>列表数据绑定对象</td>
<td>列表展示数据</td>
<td style="text-align: center;">array</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td colspan="5">搜索条件配置</td>
</tr>
<tr>
<td>查询字段名称</td>
<td>字段显示名称</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>查询字段绑定对象</td>
<td>字段绑定变量</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>使用的组件</td>
<td>该条件所用的组件</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&nbsp;</td>
<td style="text-align: center;">&nbsp;</td>
</tr>
<tr>
<td colspan="5">按钮配置</td>
</tr>
<tr>
<td>配置列表上的工具栏按钮</td>
<td>具体配置参考按钮组件配置</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td colspan="5">列配置</td>
</tr>
<tr>
<td>配置列表每列属性&nbsp;</td>
<td>具体可参考列表组件中的列配置</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>宽度改变</td>
<td>大小变化时触发</td>
<td style="text-align: center;">列表高度</td>
</tr>
<tr>
<td>查询按钮</td>
<td>查询按钮触发的事件</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>清除按钮</td>
<td>清空按钮触发事件</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>列表选中改变</td>
<td>选择数据变化时触发</td>
<td style="text-align: center;">选中数据</td>
</tr>
<tr>
<td>每页条数改变</td>
<td>每页数量变化时触发</td>
<td style="text-align: center;">每页条数</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**标签宽度**<br>
搜索条件标签文字的宽度
<br><br>

**当前页绑定对象**<br>
当前页数，支持 .sync 修饰符
<br><br>

**每页数据量绑定对象**<br>
每页显示条目个数，支持 .sync 修饰符
<br><br>

**数据总数绑定对象**<br>
总条目数
<br><br>

**列表名称**<br>
列表的名称
<br><br>

**列表数据绑定对象**<br>
显示的数据
<br><br>

**搜索条件配置**<br>
查询字段名称，查询字段对象使用的组件
<br><br>

**按钮配置**<br>
具体配置与按钮组件配置一致
<br><br>

**列配置**<br>
具体配置与列表一致
<br><br>

**事件**<br>
* 宽度改变：在宽度改变时触发的事件
* 查询按钮：在点击查询按钮时触发的事件
* 清除按钮：在点击清除按钮时触发的事件
* 列表选中改变：在列表选中改变时触发的事件
* 每页条数改变：在每条页数改变时触发的事件
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->

## ecidi选部门
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>宽度</td>
<td>组件宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>标签</td>
<td>组件标签</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">ecidi-org-selector/fawkes-org-selector</td>
<td style="text-align: center;">fawkes-org-selector</td>
</tr>
<tr>
<td>部门id绑定字段</td>
<td>部门编号绑定字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>部门名称绑定字段</td>
<td>部门名称绑定字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>请求服务器地址</td>
<td>请求服务器地址 例：http://10.215.136.245:17200</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>请求路径</td>
<td>请求接口路径 如：/sys-user/users/search</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>部门框请求路径</td>
<td>部门框请求接口路径 如：/sys-user/org/tree</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>请求参数对象</td>
<td>请求时的参数</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>部门框请求参数</td>
<td>部门框请求时的参数</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否多选</td>
<td>是否多选</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>禁用</td>
<td>是否禁用</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>是否收缩隐藏多选值</td>
<td>多选时是否将选中值按文字的形式展示</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**宽度**<br>
组件的宽度
<br><br>

**标签**<br>
组件标签名称
<br><br>

**部门id绑定字段**<br>
部门id绑定字段：deptId
<br><br>

**部门名称绑定字段**<br>
部门名称绑定字段：deptName
<br><br>

**请求服务器地址**<br>
请求的服务器地址，如：http://10.215.136.245:17200
<br><br>

**请求路径**<br>
请求的路径，如：/sys-user/users/search
<br><br>

**部门框请求路径**<br>
部门框请求的路径，如：/sys-user/org/tree
<br><br>

**请求参数对象**<br>
请求时附加参数
<br><br>

**部门框请求参数**<br>
部门框请求的参数
<br><br>

**是否多选**<br>
* 是否可多选
* 多选上限：最多能多选个数
<br><br>

**操作属性**<br>
* 禁用：是否禁用
* 只读：是否只读
* 是否收缩隐藏多选值：是否收缩隐藏多选值
<br><br>

**校验**<br>
* 必填：输入框是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**事件**<br>
值改变事件：值改变事件时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->


## ecidi选人
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>宽度</td>
<td>组件宽度</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>标签</td>
<td>组件标签</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">ecidi-org-selector/fawkes-org-selector</td>
<td style="text-align: center;">fawkes-org-selector</td>
</tr>
<tr>
<td>用户名绑定字段</td>
<td>用户名绑定字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>用户姓名绑定字段</td>
<td>用户姓名绑定字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>请求服务器地址</td>
<td>请求服务器地址 例：http://10.215.136.245:17200</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>请求路径</td>
<td>请求接口路径 如：/sys-user/users/search</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>部门框请求路径</td>
<td>部门框请求接口路径 如：/sys-user/org/tree</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>请求参数对象</td>
<td>请求时的参数</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>部门框请求参数</td>
<td>部门框请求时的参数</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否多选</td>
<td>是否多选</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>禁用</td>
<td>是否禁用</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
<tr>
<td>是否收缩隐藏多选值</td>
<td>多选时是否将选中值按文字的形式展示</td>
<td style="text-align: center;">boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">FALSE</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**宽度**<br>
组件的宽度
<br><br>

**标签**<br>
组件标签名称
<br><br>

**用户名绑定字段**<br>
用户名绑定字段：userName
<br><br>

**用户姓名绑定字段**<br>
用户姓名绑定字段：userFullName
<br><br>

**请求服务器地址**<br>
请求的服务器地址，如：http://10.215.136.245:17200
<br><br>

**请求路径**<br>
请求的路径，如：/sys-user/users/search
<br><br>

**部门框请求参数**<br>
部门框请求的参数
<br><br>

**是否多选**<br>
* 是否可多选
* 多选上限：最多能多选个数
<br><br>

**操作属性**<br>
* 禁用：是否禁用
* 只读：是否只读
* 是否收缩隐藏多选值：是否收缩隐藏多选值
<br><br>

**校验**<br>
* 必填：输入框是否必须填写，触发时机“失焦”或“值改变”
* 输入框：验证不通过时的提示信息
<br><br>

**事件**<br>
值改变事件：值改变事件时触发
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->


## ecidi范围日期
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>开始时间绑定对象</td>
<td>开始时间绑定变量</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>结束时间绑定对象</td>
<td>结束时间绑定变量</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>格式</td>
<td>日期格式</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">yyyy-MM-dd HH:mm:ss<br />yyyy-MM-dd<br />等</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**开始时间绑定对象**<br>
开始时间绑定对象：startTime
<br><br>

**结束时间绑定对象**<br>
结束时间绑定对象：endTime
<br><br>

**格式**<br>
可选日期显示的格式，如：yyyy-MM-dd
<br><br>

**操作属性**<br>
* 禁用：是否禁用
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->

## ecidi附件上传
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>标签</td>
<td>组件标签</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;" width="229">ecidi-upload<br />form-upload</td>
<td style="text-align: center;">ecidi-upload</td>
</tr>
<tr>
<td>上传地址</td>
<td>上传的地址</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>最大上传数</td>
<td>最大允许上传个数</td>
<td style="text-align: center;">number</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>文件类型</td>
<td>接受上传的文件类型（thumbnail-mode 模式下此参数无效）</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>上传的文件列表对象</td>
<td>上传的文件字段名</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>额外参数</td>
<td>上传时附带的额外参数</td>
<td style="text-align: center;">object</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>禁用&nbsp;&nbsp;</td>
<td>禁用&nbsp;</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>多文件上传</td>
<td>是否支持多选文件</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>是否显示文件列表</td>
<td>是否显示已上传文件列表</td>
<td style="text-align: center;">Boolean</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<br><br>

<table width="977">
<tbody>
<tr>
<td style="text-align: center;" width="262">事件</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">回调参数</td>
</tr>
<tr>
<td>上传前</td>
<td width="414">上传文件之前的钩子，参数为上传的文件，<br />若返回 false 或者返回 Promise 且被 reject，则停止上传。</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>上传成功</td>
<td>文件上传成功时的钩子</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>上传失败</td>
<td>文件上传失败时的钩子</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>预览</td>
<td>点击文件列表中已上传的文件时的钩子</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>删除时</td>
<td>文件列表移除文件时的钩子</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>删除前</td>
<td width="414">删除文件之前的钩子，参数为上传的文件和文件列表，<br />若返回 false 或者返回 Promise 且被 reject，则停止删除。</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>超出限制</td>
<td>文件超出个数限制时的钩子</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>

<!--

<h3>常用配置</h3><br>

**标签**<br>
组件标签名称
<br><br>

**上传地址**<br>
上传地址，如：/oa/sys-storage/upload
<br><br>

**最大上传数**<br>
限制文件最大上传数量，如'3'
<br><br>

**文件类型**<br>
文件的后缀名，多种类型以逗号分隔，如'.jpg'，'.doc'
<br><br>

**额外参数**<br>
上传时附带的额外参数
<br><br>

**操作属性**<br>
* 禁用：组件是否禁用
* 多文件上传：是否多文件上传
* 是否显示文件列表：是否显示上传的文件

**事件**<br>
* 上传前：在上传前触发的事件
* 上传成功：在上传成功时触发的事件
* 上传失败：在上传失败时触发的事件
* 预览：在预览时触发的事件
* 删除时：在删除时触发的事件
* 删除前：在删除前触发的事件
* 超出限制：在超出限制时触发的事件
<br><br>

**其他配置**<br>
用于添加非常用/自定义的属性及属性值
<br><br>

-->

## ecidi审批意见列表
***

<table width="1359">
<tbody>
<tr>
<td style="text-align: center;" width="262">属性</td>
<td style="text-align: center;" width="414">说明</td>
<td style="text-align: center;" width="301">类型</td>
<td style="text-align: center;" width="229">可选值</td>
<td style="text-align: center;" width="153">默认值</td>
</tr>
<tr>
<td>展示数组对象</td>
<td>表单评论信息</td>
<td style="text-align: center;">array</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td colspan="5">字段映射</td>
</tr>
<tr>
<td>唯一标识</td>
<td>表单上映射到唯一标识的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>处理人用户名</td>
<td>表单上映射到处理人用户名的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>处理人姓名</td>
<td>表单上映射到处理人姓名的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>流程节点名称</td>
<td>表单上映射到流程节点名称的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>签名状态</td>
<td>表单上映射到签名状态的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>处理日期</td>
<td>表单上映射到处理日期的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>评论内容</td>
<td>表单上映射到评论内容的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
<tr>
<td>流程状态标记</td>
<td>表单上映射到流程状态标记的字段</td>
<td style="text-align: center;">string</td>
<td style="text-align: center;">&mdash;</td>
<td style="text-align: center;">&mdash;</td>
</tr>
</tbody>
</table>
