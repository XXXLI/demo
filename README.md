<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>测试网页1</title>
    <link rel="stylesheet" href="bootstrap.min.css">
    <link rel="stylesheet" href="test1.css">
    <style type="text/css">
#close{ 
	background:url(img/close.png) no-repeat; 
	width:30px; 
	height:30px; 
	cursor:pointer; 
	position:absolute; 
	right:5px; 
	top:15px; 
	text-indent:-999em;
	}
#mask{ 
	background-color:#ccc;
	opacity:0.5;
	filter: alpha(opacity=50); 
	position:absolute; 
	left:0;
	top:0;
	z-index:1000;
	}
#login{ 
	position:fixed;
	z-index:1001;
	}
.loginCon{ 
	position:relative; 
	width:670px;
	height:380px;
	background:url(img/loginBg.png) #2A2C2E center center no-repeat;
	}
</style>

<script>
function openNew(){
	//获取页面的高度和宽度
	var sWidth=document.body.scrollWidth;
	var sHeight=document.body.scrollHeight;
	
	//获取页面的可视区域高度和宽度
	var wHeight=document.documentElement.clientHeight;
	
	var oMask=document.createElement("div");
		oMask.id="mask";
		oMask.style.height=sHeight+"px";
		oMask.style.width=sWidth+"px";
		document.body.appendChild(oMask);
	var oLogin=document.createElement("div");
		oLogin.id="login";
		oLogin.innerHTML="<div class='loginCon'><div id='close'>点击关闭</div></div>";
		document.body.appendChild(oLogin);
	
	//获取登陆框的宽和高
	var dHeight=oLogin.offsetHeight;
	var dWidth=oLogin.offsetWidth;
		//设置登陆框的left和top
		oLogin.style.left=sWidth/2-dWidth/2+"px";
		oLogin.style.top=wHeight/2-dHeight/2+"px";
	//点击关闭按钮
	var oClose=document.getElementById("close");
	
		//点击登陆框以外的区域也可以关闭登陆框
		oClose.onclick=oMask.onclick=function(){
					document.body.removeChild(oLogin);
					document.body.removeChild(oMask);
					};
					};
					
	window.onload=function(){
			var oBtn=document.getElementById("btnLogin");
				//点击登录按钮
				oBtn.onclick=function(){
					openNew();
					return false;
					}
				
		}
</script>
</head>
<body class="home">
<header class="main-header">
<div class="container">
<div class="row">
<div class="col-md-12">
<h1><a class="branding" href="C:\Users\Administrator\Desktop\我才是临时文件好吗\图片\火女.jpg" title="点我就给你看DOTA性感火女">DOTA是一款好玩的游戏
	<img src="C:\Users\Administrator\Desktop\我才是临时文件好吗\图片\哈尔.gif" alt="就一个简单的头部元素">
</a>
</h1>

<div id="login-area">
      <button id="btnLogin" hidefocus="true" class="login-btn">登录</button>
    </div>

</div>
	
</div>
	
</div>
</header>
<nav class="main-navigation">
<div class="container">
	<div class="row">
		<div class="col-md-12">
		<div class="navbar-header">
			<span class="nav-toggle-button collapse" data-target="#main-menu">
				<span class="sr-onlu">toggle navigation</span>
					<i class="fa fa-bars"></i>
				</span>
		</div>
			<div class="collapse navbar-collapse" id="main-menu">
				<ul class="menu">
					<li class="nav-current" role="presentation">
						<a href="#" title="别看了，这就是首页">首页</a>
					</li>
					<li role="presentation">
						<a href="http://www.dota2.com.cn/heroes/index.htm">英雄</a>
					</li>
					<li role="presentation">
						<a href="http://www.dota2.com.cn/items/index.htm">物品</a>
					</li>
					<li role="presentation">
						<a href="http://dotamax.com/">数据</a>
					</li>
					<li role="presentation">
						<a href="http://www.dota2.com.cn/info/index.htm">资料</a>
					</li>
					<li role="presentation">
						<a href="http://www.dota2.com.cn/download/">下载</a>
					</li>
				</ul>
			</div>
		</div>
	</div>
</div>
</nav>
<section class="content-warp">
	<div class="container">
	<div class="row">
		<main class="col-md-8">
			<article class="a2">
			<div class="a2-head">
			<h1 class="a2-title">
			<a href="#">啦啦啦阿拉了</a></h1>
			<div class="a2-pete">
			<span class="author">
			作者: <a href="#">小短</a> •</span>
				<time class="data" datatime="">2009年4月17日<time>	
			</div>
			</div>
			<div class="a3">
			<p>爱的精灵王到敬爱是来得及阿斯兰的空间按鹿鼎记爱上鹿鼎记</p>	
			</div>
			<div class="a4">
			<a href="#" class="btn btn-default">阅读全文</a>
			<div class="a2-footer">
			<hr>
			<div class="pull-left tag-list">
			<i class="fa fa-folder-open-o"></i>
			<a href="#">卫鸟的  ,</a>
			<a href="#">的,</a>
			<a href="#">我</a>	
			</div>
				
			</div>
				
			</div>
				
			</article>
			<article class="a2">
			<div class="a2-head">
			<h1 class="a2-title">
			<a href="#">啦啦啦阿拉了</a></h1>
			<div class="a2-pete">
			<span class="author">
			作者: <a href="#">小短</a> •</span>
				<time class="data" datatime="">2009年4月17日<time>	
			</div>
			</div>
			<div class="a3">
			<p>爱的精灵王到敬爱是来得及阿斯兰的空间按鹿鼎记爱上鹿鼎记</p>	
			</div>
			<div class="a4">
			<a href="#" class="btn btn-default">阅读全文</a>
			<div class="a2-footer">
			<hr>
			<div class="pull-left tag-list">
			<i class="fa fa-folder-open-o"></i>
			<a href="#">卫鸟的  ,</a>
			<a href="#">的,</a>
			<a href="#">我</a>	
			</div>
				
			</div>
				
			</div>
				
			</article>
			<article class="a2">
			<div class="a2-head">
			<h1 class="a2-title">
			<a href="#">啦啦啦阿拉了</a></h1>
			<div class="a2-pete">
			<span class="author">
			作者: <a href="#">小短</a> •</span>
				<time class="data" datatime="">2009年4月17日<time>	
			</div>
			</div>
			<div class="a3">
			<p>爱的精灵王到敬爱是来得及阿斯兰的空间按鹿鼎记爱上鹿鼎记</p>	
			</div>
			<div class="a4">
			<a href="#" class="btn btn-default">阅读全文</a>
			<div class="a2-footer">
			<hr>
			<div class="pull-left tag-list">
			<i class="fa fa-folder-open-o"></i>
			<a href="#">卫鸟的  ,</a>
			<a href="#">的,</a>
			<a href="#">我</a>	
			</div>
				
			</div>
				
			</div>
				
			</article>
		</main>
		<aside class="col-md-4 sidbar">
		<div class="widget">
		<h4 class="title">社区</h4>
		<div class="content community">
		<p>QQ:767618860</p>
		<p>
			<a href="#">问答社区</a>
		</p>
		<p>
			<a href="#">微博</a>
		</p>
		</div>
		</div>
		<div class="widget">
			<h4 class="title">下载</h4>
			<div class="cotent download">
			<a href="#" class="btn btn-default btn-block">中文版（0.059）</a>
				
			</div>
				
			</div>
			<div class="widget">
				<h4 class="title">标签云</h4>
				<div class="content tag-could">
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
				</div>
			</div>
			
		</aside>
	</div>
		
	</div>
		
</section>
<footer class="ft">
	<div class="container">
	<div class="row">
		<div class="col-md-4">
			<div class="ft-1">
			    <h4>最新文章</h4>
			<a href="#" class="ft-a">三大不留点已经没机会了</a>
			<p>2009年7月24日</p>
				
			<a href="#" class="ft-a">三大不留点已经没机会了</a>
			<p>2009年7月24日</p>
			   
			<a href="#" class="ft-a">三大不留点已经没机会了</a>
			<p>2009年7月24日</p>
			</div>
		</div>
		<div class="col-md-4">
			<div class="ft-2">
			<h4>又是标签云</h4>
				<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
					<a href="">59</a>
			</div>
		</div>
		<div class="col-md-4">
		<div class="ft-3">
			<h4>合作伙伴</h4>
			<a href="#">阿里云</a>
			<a href="#">新浪云</a>
			<a href="#">管你什么云</a>
			<a href="#">老子是马云</a><br>
			<a href="#">阿里云</a>
			<a href="#">新浪云</a>
			<a href="#">管你什么云</a>
			<a href="#">老子是马云</a>
			</div>
		</div>
	</div>
		
	</div>
</footer>
</body>
</html>
