# 开发报告

开发灵感
---
>   我做的网站的内容是关于《地下城与勇士》（简称DNF）的，因为我本人比较喜欢玩DNF，所以我想把DNF一些精彩有趣的东西分享给大家，让不了解DNF的同学领略一下DNF的魅力。内容中包括的图片，文字都是我在网上找到的，由于我的水平实在有限，做得不好请不要嗤笑。
页面结构
---
 >* 本站点由首页、剧情介绍、使徒介绍、角色介绍（列表页）、鬼剑士（详细页）、关于DNF（表单页）组成。  
  >* 剧情介绍、使徒介绍和角色介绍负责向游客展示DNF的剧情梗概、关键角色以及玩家所使用的角色信息。  
  >* 鬼剑士页面则是对鬼剑士这一角色的进一步介绍，让游客更加了解鬼剑士这一角色。  
  >* 最后的表单页是一份调查问卷，是我提的一些关于DNF的问题。
技术指标
---
 >  兼容的浏览器版本有IE9及以上，所用的html有部分html5的内容，所用的CSS中也有部分CSS3中的内容。
 
>开发工具：
 >>* 浏览器：Chorm、Firefox
  >*  编辑器：sublime  
  >*  辅助手册：w3school
技术点说明  
---
>  &nbsp;&nbsp;&nbsp; float元素的使用：  
网页页面是由多个区块组成，各个区块之间的位置对页面的观赏性也就极为重要，对区块进行位置调整我们可以用到float元素，区块之间默认是竖直排列，加上float元素后，可以让两个区块水平排列，当然灵活运用float元素的话就可以实现多种多样的排列
>  <pre><code></code></pre>

      embed {
	     margin-right: 0px;
	     float: right;
     }
    
     #introduce {
	   width: 1000px;
       margin-left: 200px;
	   float: right;
     }

    <div id="introduce"></div>
    <embed>
  >  
>&nbsp;&nbsp;&nbsp; nav元素的使用：
当一个列表页中内容繁多,让人想找到自己想要的内容很困难的时候，导航的作用就显得尤为重要了。nav元素可以使本区块的内容链接到其它区块，再把该区块安排的页面显眼的位置，就可以实现导航作用，让该页面便于阅读。

     <nav>
		<ul>
			<li><a href="#1">鬼剑士</a></li>
			<li><a href="#2">格斗家</a></li>
			<li><a href="#3">神枪手</a></li>
			<li><a href="#4">魔法师</a></li>
			<li><a href="#5">圣职者</a></li>
			<li><a href="#6">暗夜使者</a></li>
			<li><a href="#7">女枪手</a></li>
			<li><a href="#8">男格斗家</a></li>
		</ul>
	</nav>
	nav ul li {
	  list-style: none;
	  line-height: 30px;
    }
    nav {
	  position: fixed;
    }
    nav a:hover{
       background-color: yellow;
    }
	<li id="1"><a href="guijianshi.html"><b>鬼剑士</b></a></li>
	<li id="2"><b>格斗家</b></li>
	<li id="3"><b>神枪手</b></li>
	<li id="4"><b>魔法师</b></li>
	<li id="5"><b>圣职者</b></li>
	<li id="6"><b>暗夜使者</b></li>
	<li id="7"><b>女枪手</b></li>
	<li id="8"><b>男格斗家</b></li>
>&nbsp;&nbsp;&nbsp; jquery的引用:
进入jquery之家找到自己喜爱的特效。进去之后单击查看演示，进去演示页面后，单击右键点击检查，找到iframe元素。点击后按下F2，会显示一条网址，进入该元素下的网页，查看网页源代码，找到JS特效代码及CSS。再将其改为自己的网页所需要的样子。 而主要需要搬过来的代码为script元素下的JS特效代码，以及在head代码下的link引入的css代码。

    <!DOCTYPE html>
    <html lang="zh">
    <head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"> 
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>纯js模拟时钟插件analogClock.js|DEMO_jQuery之家-自由分享jQuery、html5、css3的插件库</title>
	<link rel="stylesheet" type="text/css" href="css/normalize.css" />
	<link rel="stylesheet" type="text/css" href="css/htmleaf-demo.css">
	<style type="text/css">
		.clock{
			width: 400px;
			margin: 30px auto;
		}
	</style>
    </head>
    <body>
	<div class="htmleaf-container">
		<header class="htmleaf-header">
			<h1>纯js模拟时钟插件analogClock.js <span>An analogClock js plug that written in native javascript</span></h1>
			<div class="htmleaf-links">
				<a class="htmleaf-icon icon-htmleaf-home-outline" href="http://www.htmleaf.com/" title="jQuery之家" target="_blank"><span> jQuery之家</span></a>
				<a class="htmleaf-icon icon-htmleaf-arrow-forward-outline" href="http://www.htmleaf.com/jQuery/Layout-Interface/201705044491.html" title="返回下载页" target="_blank"><span> 返回下载页</span></a>
			</div>
		</header>
		<div class="htmleaf-content">
			<div id="clock1" class="clock"></div>
			<div id="clock2" class="clock"></div>
			<div id="clock3" class="clock"></div>
			<div id="clock4" class="clock"></div>
		</div>
	</div>
	
	<script src="js/analogClock.js"></script>
	    <script>
	        AnalogClock("clock1");//simple use
	        AnalogClock("clock2", { width: 300, bgColor: "#bf0" });//simple option
	        AnalogClock("clock3", new AnalogClockOption(200, "#eee", "#333"));//using option class to customize

	        //base on object use, returns an clock object, can do some further style controll by the returned object.
	        var opt = new AnalogClockOption(); opt.width = 100;
	        var clock = new AnalogClock("clock4", opt);
	        clock.panel.style.border = "solid 1px red";
	    </script>
    </body>
    </html>
    这是我需要的代码：<script src="js/analogClock.js"></script>
	    <script>
	        AnalogClock("clock1");//simple use
	        AnalogClock("clock2", { width: 300, bgColor: "#bf0" });//simple option
	        AnalogClock("clock3", new AnalogClockOption(200, "#eee", "#333"));//using option class to customize

	        //base on object use, returns an clock object, can do some further style controll by the returned object.
	        var opt = new AnalogClockOption(); opt.width = 100;
	        var clock = new AnalogClock("clock4", opt);
	        clock.panel.style.border = "solid 1px red";
	    </script>

   开发心得
---
   >本站点的制作非常简单，并没有复杂之处，不足的地方太多太多，主要还是因为我能力有限，不过我还是有所收获的，毕竟我做出了我的一个网站，接下来我会继续努力的！

 
  




