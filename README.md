<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>开发报告</title>
</head>
<body>
<div id="wmd-preview" class="wmd-preview"><div class="md-section-divider"></div><div class="md-section-divider"></div><h1 data-anchor-id="lf0l" id="开发报告">开发报告</h1><div class="md-section-divider"></div><h2 data-anchor-id="wqts" id="开发灵感">开发灵感</h2><blockquote data-anchor-id="8mac" class="white-blockquote">
  <p>我做的网站的内容是关于《地下城与勇士》（简称DNF）的，因为我本人比较喜欢玩DNF，所以我想把DNF一些精彩有趣的东西分享给大家，让不了解DNF的同学领略一下DNF的魅力。内容中包括的图片，文字都是我在网上找到的，由于我的水平实在有限，做得不好请不要嗤笑。</p>
</blockquote><div class="md-section-divider"></div><h2 data-anchor-id="nrl0" id="页面结构">页面结构</h2><blockquote data-anchor-id="hb0f" class="white-blockquote">
  <ul>
  <li>本站点由首页、剧情介绍、使徒介绍、角色介绍（列表页）、鬼剑士（详细页）、关于DNF（表单页）组成。  </li>
  <li>剧情介绍、使徒介绍和角色介绍负责向游客展示DNF的剧情梗概、关键角色以及玩家所使用的角色信息。  </li>
  <li>鬼剑士页面则是对鬼剑士这一角色的进一步介绍，让游客更加了解鬼剑士这一角色。  </li>
  <li>最后的表单页是一份调查问卷，是我提的一些关于DNF的问题。</li>
  </ul>
</blockquote><div class="md-section-divider"></div><h2 data-anchor-id="fjlz" id="技术指标">技术指标</h2><blockquote data-anchor-id="1ewy" class="white-blockquote">
  <p>兼容的浏览器版本有IE9及以上，所用的html有部分html5的内容，所用的CSS中也有部分CSS3中的内容。</p>
  
  <p>开发工具：</p>
  
  <blockquote class="white-blockquote">
    <ul>
    <li>浏览器：Chorm、Firefox</li>
    <li>编辑器：sublime  </li>
    <li>辅助手册：w3school</li>
    </ul>
  </blockquote>
</blockquote><div class="md-section-divider"></div><h2 data-anchor-id="6gkl" id="技术点说明">技术点说明  </h2><blockquote data-anchor-id="dciq" class="white-blockquote">
  <p>&nbsp;&nbsp;&nbsp; float元素的使用： <br>
  网页页面是由多个区块组成，各个区块之间的位置对页面的观赏性也就极为重要，对区块进行位置调整我们可以用到float元素，区块之间默认是竖直排列，加上float元素后，可以让两个区块水平排列，当然灵活运用float元素的话就可以实现多种多样的排列 <br>
 </p><pre><code></code></pre><p></p>
</blockquote><pre data-anchor-id="skq0"><code>  embed {
     margin-right: 0px;
     float: right;
 }

 #introduce {
   width: 1000px;
   margin-left: 200px;
   float: right;
 }

&lt;div id="introduce"&gt;&lt;/div&gt;
&lt;embed&gt;
</code></pre><blockquote data-anchor-id="bbo0" class="white-blockquote">
  <p>&nbsp;&nbsp;&nbsp; nav元素的使用： <br>
  当一个列表页中内容繁多,让人想找到自己想要的内容很困难的时候，导航的作用就显得尤为重要了。nav元素可以使本区块的内容链接到其它区块，再把该区块安排的页面显眼的位置，就可以实现导航作用，让该页面便于阅读。</p>
</blockquote><pre data-anchor-id="2hsr"><code> &lt;nav&gt;
    &lt;ul&gt;
        &lt;li&gt;&lt;a href="#1"&gt;鬼剑士&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#2"&gt;格斗家&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#3"&gt;神枪手&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#4"&gt;魔法师&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#5"&gt;圣职者&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#6"&gt;暗夜使者&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#7"&gt;女枪手&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#8"&gt;男格斗家&lt;/a&gt;&lt;/li&gt;
    &lt;/ul&gt;
&lt;/nav&gt;
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
&lt;li id="1"&gt;&lt;a href="guijianshi.html"&gt;&lt;b&gt;鬼剑士&lt;/b&gt;&lt;/a&gt;&lt;/li&gt;
&lt;li id="2"&gt;&lt;b&gt;格斗家&lt;/b&gt;&lt;/li&gt;
&lt;li id="3"&gt;&lt;b&gt;神枪手&lt;/b&gt;&lt;/li&gt;
&lt;li id="4"&gt;&lt;b&gt;魔法师&lt;/b&gt;&lt;/li&gt;
&lt;li id="5"&gt;&lt;b&gt;圣职者&lt;/b&gt;&lt;/li&gt;
&lt;li id="6"&gt;&lt;b&gt;暗夜使者&lt;/b&gt;&lt;/li&gt;
&lt;li id="7"&gt;&lt;b&gt;女枪手&lt;/b&gt;&lt;/li&gt;
&lt;li id="8"&gt;&lt;b&gt;男格斗家&lt;/b&gt;&lt;/li&gt;
</code></pre><blockquote data-anchor-id="j38d" class="white-blockquote">
  <p>&nbsp;&nbsp;&nbsp; jquery的引用: <br>
  进入jquery之家找到自己喜爱的特效。进去之后单击查看演示，进去演示页面后，单击右键点击检查，找到iframe元素。点击后按下F2，会显示一条网址，进入该元素下的网页，查看网页源代码，找到JS特效代码及CSS。再将其改为自己的网页所需要的样子。 而主要需要搬过来的代码为script元素下的JS特效代码，以及在head代码下的link引入的css代码。</p>
</blockquote><pre data-anchor-id="7rey"><code>&lt;!DOCTYPE html&gt;
&lt;html lang="zh"&gt;
&lt;head&gt;
&lt;meta charset="UTF-8"&gt;
&lt;meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"&gt; 
&lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;
&lt;title&gt;纯js模拟时钟插件analogClock.js|DEMO_jQuery之家-自由分享jQuery、html5、css3的插件库&lt;/title&gt;
&lt;link rel="stylesheet" type="text/css" href="css/normalize.css" /&gt;
&lt;link rel="stylesheet" type="text/css" href="css/htmleaf-demo.css"&gt;
&lt;style type="text/css"&gt;
    .clock{
        width: 400px;
        margin: 30px auto;
    }
&lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;div class="htmleaf-container"&gt;
    &lt;header class="htmleaf-header"&gt;
        &lt;h1&gt;纯js模拟时钟插件analogClock.js &lt;span&gt;An analogClock js plug that written in native javascript&lt;/span&gt;&lt;/h1&gt;
        &lt;div class="htmleaf-links"&gt;
            &lt;a class="htmleaf-icon icon-htmleaf-home-outline" href="http://www.htmleaf.com/" title="jQuery之家" target="_blank"&gt;&lt;span&gt; jQuery之家&lt;/span&gt;&lt;/a&gt;
            &lt;a class="htmleaf-icon icon-htmleaf-arrow-forward-outline" href="http://www.htmleaf.com/jQuery/Layout-Interface/201705044491.html" title="返回下载页" target="_blank"&gt;&lt;span&gt; 返回下载页&lt;/span&gt;&lt;/a&gt;
        &lt;/div&gt;
    &lt;/header&gt;
    &lt;div class="htmleaf-content"&gt;
        &lt;div id="clock1" class="clock"&gt;&lt;/div&gt;
        &lt;div id="clock2" class="clock"&gt;&lt;/div&gt;
        &lt;div id="clock3" class="clock"&gt;&lt;/div&gt;
        &lt;div id="clock4" class="clock"&gt;&lt;/div&gt;
    &lt;/div&gt;
&lt;/div&gt;

&lt;script src="js/analogClock.js"&gt;&lt;/script&gt;
    &lt;script&gt;
        AnalogClock("clock1");//simple use
        AnalogClock("clock2", { width: 300, bgColor: "#bf0" });//simple option
        AnalogClock("clock3", new AnalogClockOption(200, "#eee", "#333"));//using option class to customize

        //base on object use, returns an clock object, can do some further style controll by the returned object.
        var opt = new AnalogClockOption(); opt.width = 100;
        var clock = new AnalogClock("clock4", opt);
        clock.panel.style.border = "solid 1px red";
    &lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;
这是我需要的代码：
   &lt;script src="js/analogClock.js"&gt;&lt;/script&gt;
    &lt;script&gt;
        AnalogClock("clock1");//simple use
        AnalogClock("clock2", { width: 300, bgColor: "#bf0" });//simple option
        AnalogClock("clock3", new AnalogClockOption(200, "#eee", "#333"));//using option class to customize

        //base on object use, returns an clock object, can do some further style controll by the returned object.
        var opt = new AnalogClockOption(); opt.width = 100;
        var clock = new AnalogClock("clock4", opt);
        clock.panel.style.border = "solid 1px red";
    &lt;/script&gt;
</code></pre><div class="md-section-divider"></div><h2 data-anchor-id="cxd0" id="开发心得">   开发心得</h2><blockquote data-anchor-id="hcf0" class="white-blockquote">
  <p>本站点的制作非常简单，并没有复杂之处，不足的地方太多太多，主要还是因为我能力有限，不过我还是有所收获的，毕竟我做出了我的一个网站，接下来我会继续努力的！</p>
</blockquote></div>
</body>
</html>