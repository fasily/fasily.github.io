---
layout: page
title: 刘旭东
tagline: —认真做自己
---
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<link rel="stylesheet" type="text/css" media="all" href="style.css">
<script language="javascript" type="text/javascript" src="js/js.js"></script>
<script type="text/javascript" src="http://code.jquery.com/jquery-1.6.4.min.js"></script>
<title>刘旭东的个人主页</title>

</head>

<body>

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
<div id="photo" class="jpg">
<img src="1.jpg" alt="Drawing" width="300px" />
</div>
<div id="describe" >
<br>
大家好,我是刘旭东，期待与大家交流，享受分享的快乐。现在我是北京理工大学的一名在读硕士，2015年毕业。热爱机器学习、数据挖掘，享受C++的博大精深，深知开源的力量，看好互联网的前景。
喜欢看NBA，Huston Rockets的支持者，热爱运动，篮球、羽毛球、乒乓球都比较喜欢，水平一般般。现在的我在不断给自己充电，希望自己不断生根发芽。
</div>

</body>


