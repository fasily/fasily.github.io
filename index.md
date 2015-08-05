---
layout: page
title: 刘旭东
tagline: —知人者智，自知者明。胜人者有力，自胜者强。
---

<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<link rel="stylesheet" type="text/css" media="all" href="style.css">
<script language="javascript" type="text/javascript" src="js/js.js"></script>
<script type="text/javascript" src="http://code.jquery.com/jquery-1.6.4.min.js"></script>
<title>刘旭东的个人主页</title>
<script type="text/javascript">
$(document).ready(function() {

	// 创建两个变量，一个数组中的月和日的名称
	var monthNames = [ "一月", "二月", "三月", "四月", "五月", "六月", "七月", "八月", "九月", "十月", "十一月", "十二月" ]; 
	var dayNames= ["星期日","星期一","星期二","星期三","星期四","星期五","星期六"]

	// 创建一个对象newDate（）
	var newDate = new Date();
	// 提取当前的日期从日期对象
	newDate.setDate(newDate.getDate());
	//输出的日子，日期，月和年
	$('#Date').html(newDate.getFullYear() + " " + monthNames[newDate.getMonth()] + ' ' + newDate.getDate() + ' ' + dayNames[newDate.getDay()]);

	setInterval( function() {
		// 创建一个对象，并提取newDate（）在访问者的当前时间的秒
		var seconds = new Date().getSeconds();
		//添加前导零秒值
		$("#sec").html(( seconds < 10 ? "0" : "" ) + seconds);
	},1000);
	
	setInterval( function() {
		// 创建一个对象，并提取newDate（）在访问者的当前时间的分钟
		var minutes = new Date().getMinutes();
		// 添加前导零的分钟值
		$("#min").html(( minutes < 10 ? "0" : "" ) + minutes);
    },1000);
	
	setInterval( function() {
		// 创建一个对象，并提取newDate（）在访问者的当前时间的小时
		var hours = new Date().getHours();
		// 添加前导零的小时值
		$("#hours").html(( hours < 10 ? "0" : "" ) + hours);
    }, 1000);
	
}); 
</script>
</head>

<body>
<div id="right">
<div class="clock" style="align=center;">
	<div id="Date"></div>
	<ul>
		<li id="hours" > </li>
		<li id="point">:</li>
		<li id="min"> </li>
		<li id="point">:</li>
		<li id="sec"> </li>
	</ul>
</div>
<div id="myblogtext">
<h2>我的随笔：</h2><br>
<ul> 
<li>1 Aug 2015 >> <a href="/sb/2015/08/01/hw">用心等待</a></li>
</ul>
</div>
</div>
<div id="myself">
<div id="photo" class="jpg">
<img src="1.jpg" alt="Drawing" width="300px" />
</div>
<div id="describe" style="font-size:15px">
<br>
大家好,我是刘旭东，2015年北京理工大学硕士毕业，现在就职于大唐电信集团旗下高鸿股份公司。热爱机器学习、数据挖掘，享受工程实践带来的乐趣，希望在互联网+时代实现自己的价值。
喜欢看NBA，Huston Rockets的支持者，热爱运动，篮球、羽毛球、乒乓球都比较喜欢，坚信身体是革命的本钱。期待与大家交流，享受分享的快乐。
</div>
</div>
<div id="myblogtext">
<h2>我的博文：</h2><br>
<ul> 
<li>24 Dec 2014 >> <a href="/statistic/2014/12/28/markov">马尔科夫链</a></li>
<li>24 Dec 2014 >> <a href="http://www.cnblogs.com/retarded/articles/4129413.html">EM算法介绍</a></li>
</ul>

</div>
</body>


