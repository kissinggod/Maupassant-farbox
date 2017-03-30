# ReadMe

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
<script src="https://use.typekit.net/rnh3yip.js"></script>
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
            border-radius:5px;
    }
     
    .post-content img:hover{
          border-radius:5px;
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
      border-radius:5px;
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
</style>
```