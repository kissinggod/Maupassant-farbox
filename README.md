# ReadMe

## 重要声明

本Mod不适配IE浏览器，未来也不会适配。用IE浏览器会出现部分功能或视觉效果出错的问题，建议使用Safari、Chrome等浏览器。

##  Maupassant for Bitcron Mod v1.5

### 改进
- 部分支持（去除了链接、标题等常见元素的样式）Bootstrap样式（需在站点后台-呈现-嵌入模板中更新设置，更新后的代码在下方）
- 完全支持FontAwesome

### 新增功能
- 添加主页，可通过在站点根目录下创建`index.md`文件自行增加
- 添加关于页面，可通过在站点根目录下创建`about.md`文件自行增加[^1]

### 微调
- 更改博客页面头部站点标题字体及颜色
- 博客页面头部增加站点描述/副标题

## Maupassant for Bitcron Mod v1.2

### 微调
- 更改博文超链接样式
- 更改导航栏超链接悬停样式

### 改进
- 解决中尺寸屏幕（iPad或iPad Mini）在竖屏状态下，文章右侧出现大量空白的问题

## Maupassant for Bitcron Mod v1.1

### 修复
- 修复标签功能失效的问题
- 修复背景图不显示的问题
- 修复搜索功能失效的问题
- 修复评论时间不显示的问题

### 改进
- 改进在小屏幕上评论宽度溢出容器的问题 <del>（将在下一个版本中重制评论系统样式，彻底解决这个问题）</del>


## Maupassant for Bitcron Mod v1.0

原作者：[Cho](https://github.com/pagecho)
原项目地址：https://github.com/pagecho/Maupassant-farbox

Maupassant是Cho为原Farbox平台开发的一款主题，其设计简洁雅致。近日，随着Bitcron的升级，Maupassant完成了对该平台的适配（但我没找到项目地址……）。

按惯例，根据自己的使用习惯稍微修改了一下，主要改动如下：

### 功能

- 增加文章密码保护功能
- 增加文章摘要功能`class:.intro`
- 增加文章页签名档
- 增加文章页导航按钮

### 样式

- 字体替换成`思源黑体`和`Monarcha`组合
- 微调配色方案
- 修改强调样式（加粗）
- 修改脚注样式`Bigfoot.js`
- 增加图注、左对齐、右对齐、图注对齐及花式引用样式
- 增加全站背景图

### 细节

- 图片和按钮取消圆角，以令整体设计更协调
- 增加自适应设计，在手机上浏览时，超出元素宽度的表格及导航栏隐藏
- 所有输入框底色调整为透明

以上。具体效果可参考[**示例页面**](http://bit.lanieldev.com/post/webkai-fa/lorem2)。

注：需要在Bitcron网站后台的「呈现」面板中添加以下代码：

```
<link rel="stylesheet" href="/template/style.scss">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="stylesheet" href="/template/bootstrap2.css">

<style>
.site_nav:hover{
color: #DC317F !important;
}

.nav__item{
font-size:13px;
}

.nav__item:hover{
		color: #DC317F !important;
		}

@-webkit-keyframes fadeIn {
0% {
opacity: 0; /*初始状态 透明度为0*/
}
50% {
opacity: 0; /*中间状态 透明度为0*/
}
100% {
opacity: 1; /*结尾状态 透明度为1*/
}
}

.zzsc {
	-webkit-transition: -webkit-transform 2s ease-out;
	-moz-transition: -moz-transform 2s ease-out;
	-o-transition: -o-transform 2s ease-out;
	-ms-transition: -ms-transform 2s ease-out;
	-webkit-animation-name: fadeIn; /*动画名称*/
    -webkit-animation-duration: 3s; /*动画持续时间*/
    -webkit-animation-iteration-count: 1; /*动画次数*/
    -webkit-animation-delay: 0s; /*延迟时间*/
}
.zzsc:hover {
	-webkit-transform: rotateZ(360deg);
	-moz-transform: rotateZ(360deg);
	-o-transform: rotateZ(360deg);
	-ms-transform: rotateZ(360deg);
	transform: rotateZ(360deg);
}

h3 .subtitle{
word-spacing:0.5em !important;
}

.subtitle{
display:block;
text-align:center !important;
}

.motto{
text-align:center;
font-size:1.5em!important;
margin-top:-1.5em;
}

.test123{
    display:inline;
   text-align:center;
    font-size:1em!important;
    padding: 20px 5px 0 5px;
    line-height:1;
    }


.btn-default{
color:#000  !important;
}

.btn-default:hover{
color:#de2b7f !important;
}

.introtext{
text-align:center;
color:#adadad;
}

</style>

<script src="https://use.typekit.net/（你的Typekit KitID）.js"></script>
<script>try{Typekit.load({ async: true });}catch(e){}</script>

<style>
   hide{
   color:#b7b7b7;
   background-color:#b7b7b7;
   padding:0.2em;
   }

hide:hover{
   color:#777;
   background-color:#fff;
   }

    .post-content img{
            border-radius:0;
    }
     
    .post-content img:hover{
          border-radius:0;
    }
    
    .alignright {
      float: right;
      margin: 0;
      margin-left: 25px;
    }
    
    .alignright {
      float: right;
      margin: 0;
      margin-left: 25px;
    }     
    
    .alignleft {
      float: left;
      margin: 0;
      margin-right: 25px;
    }
    
    .alingcenter{
      clear: both;
      display: block;
      margin: 0 auto;
    }
    
    div.quote{
      display:block;
      float: right;
      margin-left: 0.6em;
      margin-bottom: 0.5em;
      margin-top: 0.1em;
      max-width: 12em;
      font-size: 26px;
      color: #66747E;
      text-indent: -0.4em;
      font-family: STSong, Songti SC Light, Sonti SC, serif;
      font-weight:300;
      font-style:italic;
      background: url(/template/img/quote5.png) no-repeat;
      padding: 1.6em 0 0.2em 2em;
    }
    
    #div.quote::before {
      content: "\201C";
      font-family: source-han-sans-simplified-c, sans-serif;
      font-size: 80px;
      font-weight: bold;
      position:absolute;
      left: -40px;
      top: -20px;
    }
    
    .wp-caption{
        display: block;
          clear:both;
        height: auto;
        margin: 0 auto;
         margin-bottom: 1em;
        max-width: 100%;
    }      
    
    .wp-caption img{
         text-align:center;
         display:block;
         margin:0 auto;
        max-width: 100%;
      border-radius:0;
    }
    
    .wp-caption-text {
        -moz-box-sizing: border-box;
        box-sizing:      border-box;
        font-size: 13px;
        font-style: italic;
        line-height: 1.3076923076;
        margin: 10px 0 7px;
        padding: 0 10px 0 0; /* Avoid the caption to overflow the width of the image because wp-caption has 10px wider width */
        text-align: center;
    }  
    
    .wp-caption-alignleft{
        float: left;
         margin: 0;
         margin-right: 25px;
    }       
    
    .wp-caption-alignright{
        float: right;
         margin: 0;
         margin-left: 25px;
    }
 </style>

<style>
.toc{
border-radius:0  !important;
}

.category{
font-family:"monarcha","田氏宋体旧字形","ST Songti","source-han-sans-simplified-c","ff-tisa-web-pro", Cambria, "Times New Roman", Georgia, Times, sans-serif;
}

strong{
font-weight:bold;
}

.listing{
font-family:"monarcha","田氏宋体旧字形","ST Songti","source-han-sans-simplified-c","ff-tisa-web-pro", Cambria, "Times New Roman", Georgia, Times, sans-serif;
}
</style>

<script type="text/javascript">
    var bigfoot = $.bigfoot(
        {
            deleteOnUnhover: false,
            preventPageScroll: false,
            hoverDelay: 250
            }
        );
  </script>

<style>
 ::selection {
    background:#FCFCCF;
}

::-moz-selection {
    background:#FCFCCF;
}
table, thead, tr, th, td{
	background: transparent !important;
}
.tags a:hover{color:#DC317F !important;}
.pager a:hover{color:#DC317F !important;}
</style>
```

[^1]: 具体的创建方式可以参考Bitcron的[官方说明](https://pi.bitcron.com)，如果赶时间可以看这篇个人认为总结得相当到位的[文章](https://www.liaoyuqin.com/post/help/pibitcron)。

