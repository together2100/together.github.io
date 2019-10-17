  # Bootstrap 安装  
只需要它的样式文件， 找到dist文件夹下的css，js，font，把它们复制到你的项目里  
通过导入就可以调用了。

# Bootstrap 使用  
container 内容容器  
头部必须有 <meta name="viewport" content="width=device-width, initial-scale=1.0">  
这句代码意思是让移动设备优先。  

## 栅格  
系统最大自动分为12列  
```
<div class= "col-lg-1 ">1</div> 一行最多显示12个，多出来的会排到下一行
```
col-lg  > 1200px宽度  
col-md > 992px宽度  
col-sm > 750px宽度  
col-sx < 750px 宽度  
### col-lg-1 col-lg-2 col-lg-3 后面的数字代表占的格子数量，一行最多占12，超过的，换到下行  

## 对齐方式  
text-left 左对齐  
text-right 右对齐  
text-center居中对齐  
text-justify 超出屏幕部分自动换行  
text-nowrap 超出屏幕部分不换行  
## 设置文字  
text-lowercase 文本小写  
text-uppercase 文本大写  
text-capitalize 单词首字母大写  

## 强调文字设置  
text-muted:提示,使用浅灰色(#999)  
text-primary:主要,使用蓝色(#428bca)  
text-success:成功,使用浅绿色(#3c763d)  
text-info:通知信息,使用浅蓝色(#31708f)  
text-warning:警告,使用黄色(#8a6d3b)  
text-danger:危险,使用褐色(#a94442)  

## 浮动  
pull-left 左浮动  
pull-right 右浮动  
clearfix 清除浮动  

# 表格属性  
table-striped 斑马形式条纹（隔行变色）  
table-bordered  为所有表格的单元格添加边框？  
table-hover  在 任一行启用鼠标悬停状态  
table-condensed  让表格更加紧凑  

## tr td th
active 将悬停的颜色应用在行或者单元格上    
  success 表示成功的操作  
  info   表示信息变化的操作  
warning  表示一个警告的操作  
danger   表示一个危险的操作

#  表单
form-group 分组
form-horizontal 水平表单
control-label 

```
<form action="" role="form">
<div class="form-group">
		<label for="name">用户名：</label>
        <input type="text" class="form-control" name="name">
</div>
```
## 按钮

## 按钮组
button data-toggle = "dropdown"   
ul class = "dropdown-menu"  

## 字体图标  

## img  

## 背景  

# JS 文件引入顺序  先导入JQ，再导入JS，不然会报错。  

## 插件 模态框  
```
<button class="btn btn-success" data-target="#mymodal" data-toggle="modal">
           添加收获地址
        </button>
        <!-- 模态框主体 -->
        <div id="mymodal" class="modal"> -->
             <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <!-- data-dismiss 关闭模态框 -->
                        <button class="close" data-dismiss="modal">&times;</button>
                        <h3>添加收货地址</h3>
                    </div>
                    <div class="modal-body">
                        <form action="">
                            <div class="form-group">
                                <label for="shouhuoren">收货人</label>
                                <input type="text" class="form-control" id="shouhuoren">
                            </div>
                            <div class="form-group">
                                    <label for="tel">电话</label>
                                    <input type="text" class="form-control" id="tel">
                                </div>
                                <div class="form-group">
                                        <label for="address">地址</label>
                                        <select name="" id="address">
                                            <option value="">--请选择--</option>
                                        </select>
                                    </div>
                                    <div class="form-group">
                                        <input type="submit" value="提交" class="btn btn-success btn-block">
                                    </div>
                        </form>
                    </div>
                    <div class="modal-footer">
                        <button class="btn btn-info" data-dismiss="modal">关闭</button>
                    </div>
                </div>
            </div>
        </div>
```

# 下拉菜单  
```
<button class="btn btn-primary" data-toggle="collapse" data-target="#user">用户管理</button>
        <div id="user" class="collapsing">  collapsing是隐藏
            <li>用户列表</li>
            <li>添加用户</li>
        </div>
        <button class="btn btn-primary" data-toggle="collapse"
        data-target="#tie">帖子管理</button>
        <div id="tie" class="collapsing">
            <li>帖子列表</li>
            <li>添加帖子</li>
        </div>
```










