# sui-search

> **组件名：sui-search**
> 代码块： `sui-search`

### 安装方式

本组件符合[easycom](https://uniapp.dcloud.io/collocation/pages?id=easycom)规范，`HBuilderX 2.5.5`起，只需将本组件导入项目，在页面`template`中即可直接使用，无需在页面中`import`和注册`components`。

### 基本用法

在 ``template`` 中使用组件

```html
<!-- 基本用法 -->
<sui-search @blur="blur"></sui-search>

<!-- 初始值 -->
<sui-search :focus="true" :value="searchValue" @blur="blur"></sui-search>

<!-- 自定义placeholder -->
<sui-search placeholder="自定义placeholder" @blur="blur"></sui-search>

<!-- 设置圆角 -->
<sui-search :radius="0" @blur="blur"></sui-search>

<!-- 禁止输入-->
<sui-search :disabled="true" @gosearch="gosearch"></sui-search>
```

## API
### suiSearch Props

|属性名			|类型	|默认值	|说明																					|
|:-:			|:-:	|:-:	|:-:																					|
|value	|StringNumber	|	|搜索栏绑定值																		|
|radius			|Number	|10		|搜索栏圆角，单位px																	|
|disabled	|Boolean	|false	|是否禁止输入																|
|placeholder	|String	|	|搜索栏Placeholder																		|
|placeStyle		|String	|color:#999;font-size:24rpx;	|搜索栏Placeholder样式|
|background		|String	|#F5F5F5|输入框背景															|
|focus		|Boolean	|false	|															|

### suiSearch Events

|事件称名	|说明																|返回参数			|
|:-:		|:-:																|:-:				|
|@gosearch			|input 禁止输入时触发事件，返回参数为suiSearch的value				|e=value	|
|@blur			|input 失去焦点时触发事件，返回参数为suiSearch的value				|e=value	|

### 右侧添加 的 slot 插槽

|插槽称名	|说明|
|:-:		|:-:	|
|right	|右侧自定义插槽|
