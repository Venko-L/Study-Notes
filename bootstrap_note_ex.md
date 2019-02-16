### 简单配置

网上也有说下载的，不过事实证明找那三条链接就好了

在index.html添加

```
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@3.3.7/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/jquery@1.12.4/dist/jquery.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@3.3.7/dist/js/bootstrap.min.js"></script>
```

- 下面两行循序不能颠倒

### 视频笔记

（这部分很跳，要不是看过视频我都不知道自己写的什么。。）

（实际上有些地方已经忘了。。）

（bootstrap真是花里胡哨的，不过确实蛮好用，真香）

1.

```
<div class="container">
    <div class="row">
        <div class="col-md-6">4</div>

        <div class="col-md-6">8</div>
    </div>
</div>
```


class="col-md-4"占一行的4/12

2.
height太高把下一个同行的列挤到旁边去时，用class="clearfix"

3.
往右边移动4格 class="col-md-offset-4"

4.列的微调
class="col-md-push-4"往右	推4
class="col-md-pull-4"	拉4

5.副标题	<small></small>

6.段落添加class="lead" 样式突出

7.文字高亮显示<mark></mark>类似于``

8.删除线<del><s>同上

9.下划线<ins>同上

10.文字居中class="text-center"
类比"text-left""text-right"

11.斜体<em>同上

12.小号文字<small>

13.着重，就是变粗<strong>同上

14.无序列表、有序列表

```
<ul>
	<li></li>
	<li></li>
	<li>
		<ul>
			<li></li>
			<li></li>
			<li></li>
		</ul>
	</li>
</ul>
```


ul换成ol也一样

15.无序/有序列表的无样式class="list-unstyled"

16.带描述短语列表

```
<dl>
	<dt></dt>标题
	<dd></dd>
</dl>
```

17.水平短语列表
class="dl-horizontal"
标题和文本放在一行，上下几个都对齐了

18.类似代码块
<kbd>黑色的背景
`&lt;`相当于<
`&gt;` 相当于>
<code>相当于``

19.表单，表格形式class="table"
隔行换颜色class="table-striped"
边框class="table-bordered"

20.hover效果添加边框class="table-hover"

21.状态类设置颜色
active	鼠标悬停显示，灰色
success	绿色
info	提示信息，蓝色
warning	警告，黄色
danger	危险，红色

22.水平式响应布局 class="table-condensed"
小窗口里自动换行以适应屏宽的，变成不换行，所有东西在一行内

23.

32.单选框radio，name=“hobby”，name里面的名字必须一样，才能单选
外加label，那么点文字也能选中
disable属性，不能选（禁用）

for要对应相应id才能成为一对

disable属性可禁用text输入框

输入框只读，readonly属性

33.button状态以及颜色
class=“btn btn-default”	默认，灰白色
class=“btn btn-primary”	首选项，深蓝
class=“btn btn-success”	成功，绿色
class=“btn btn-info”	一般信息，浅蓝
class=“btn btn-warning”	警告，黄色
class=“btn btn-danger”	危险，红色

34.button大小
class=“btn btn-default btn-xs”或者sm，或者lg

35.文本背景颜色
class=“bg-info”同上

36.字体颜色
class=“text-info”同上

37.关闭按钮

```
<button type="button" class="close" >&times;</button>
```

`&times;` 为X

38.空格`&nbsp;` 

39.浮动
pull-left	左浮动
pull-right	右浮动

40.可用的类
针对不同屏幕尺寸隐藏或显示内容

41.字体图标 glyphicons

42.下拉菜单

43.下拉框分割线和不可选

44.一组按钮

45.多个按钮组

46.使用标签样式

47.盒子样式+表单样式+表格

48.模态框

### 以下为官网+视频找的些许用得上的例(板)子

- 标为可用是因为那时出了点问题，实际上全部都能用吧。。大概？

- 或者偶尔有些用不了那个效果的，找回视频就好了

  （还有个黑色的类型dark呢）

49.分类标签栏

```
<ul class="nav nav-tabs">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>
```

50.胶囊型分类标签栏

```
<ul class="nav nav-pills">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>
```

51.单按钮下拉菜单

```
<!-- Single button -->
<div class="btn-group">
  <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Action <span class="caret"></span>
  </button>
  <ul class="dropdown-menu">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>
```

52.默认分页

```
<nav aria-label="Page navigation">
  <ul class="pagination">
    <li>
      <a href="#" aria-label="Previous">
        <span aria-hidden="true">&laquo;</span>
      </a>
    </li>
    <li><a href="#">1</a></li>
    <li><a href="#">2</a></li>
    <li><a href="#">3</a></li>
    <li><a href="#">4</a></li>
    <li><a href="#">5</a></li>
    <li>
      <a href="#" aria-label="Next">
        <span aria-hidden="true">&raquo;</span>
      </a>
    </li>
  </ul>
</nav>
```

53.导航中的表单

```
<form class="navbar-form navbar-left" role="search">
  <div class="form-group">
    <input type="text" class="form-control" placeholder="Search">
  </div>
  <button type="submit" class="btn btn-default">Submit</button>
</form>
```

54.固定顶部导航栏

```
<nav class="navbar navbar-default navbar-fixed-top">
  <div class="container">
    ...
  </div>
</nav>
```

55.固定在底部

```
<nav class="navbar navbar-default navbar-fixed-bottom">
  <div class="container">
    ...
  </div>
</nav>
```

56.反色导航栏

```
<nav class="navbar navbar-inverse">
  ...
</nav>
```

57.模态框（可用）

```
<div class="modal fade" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel">
    <div class="modal-dialog" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <h4 class="modal-title" id="myModalLabel">Modal title</h4>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
          
    </div>
        <div class="modal-body">
          ...
        </div>
    <div class="modal-footer">
      <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
      <button type="button" class="btn btn-primary">Save changes</button>
    </div>
  </div>
</div>

  </div>
```

58.小模态框（可用）

```
<button type="button" class="btn btn-primary" data-toggle="modal" data-target=".bs-example-modal-sm">Small modal</button>

<div class="modal fade bs-example-modal-sm" tabindex="-1" role="dialog" aria-labelledby="mySmallModalLabel">
  <div class="modal-dialog modal-sm" role="document">
    <div class="modal-content">
      
        <div class="modal-header">
            <h4 class="modal-title" id="myModalLabel">Modal title</h4>
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>

          </div>
       <!-- ...    -->
    </div>

  </div>
</div>
```

59.按钮组（可用）


```
<div class="btn-group" role="group" aria-label="...">
      <button type="button" class="btn btn-info">修改</button>
      <button type="button" class="btn btn-success">退出</button>
      <button type="button" class="btn btn-danger">注销</button>
    </div>
```

60.表格（可用）

```
<div >
  <table class="table table-striped table-bordered table-hover">
    
    <!-- On cells (`td` or `th`) -->
    <tr class="bg-info">
        <th class="active">11</th>
        <th class="success">22</th>
        <th class="warning">33</th>
        <th class="danger">44</th>
        <th class="info">55</th>
        <th class="info">66</th>
      </tr>
    <tr>
      <td class="active">11</td>
      <td class="success">22</td>
      <td class="warning">33</td>
      <td class="danger">44</td>
      <td class="info">55</td>
      <td class="info">66</td>
    </tr>

  </table>
</div>
```



### 另外

JSON中不允许有备注，所以先放在这里吧

这个是下了bootstrap以及jquery.js之后需手动添加的内容

实际上太麻烦了直接上链接吧，放在最顶上了

我的话，加在angular.json 分别是25、28行左右吧

```
"./node_modules/bootstrap/dist/css/bootstrap.css"

"./node_modules/jquery/dist/jquery.js",
"./node_modules/bootstrap/dist/js/bootstrap.js"
```

