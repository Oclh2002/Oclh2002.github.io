<!DOCTYPE html>
 
 
<html lang="zh-CN">
 
 
 
<head>
 
<meta charset="UTF-8">
 
<meta name="viewport" content="width=device-width, initial-scale=1.0">
 
<title>武大日报平安</title>
 
<script type="text/javascript">
 
function getDate() {
 
var today = new Date();
 
 
 
var m = today.getMonth() + 1;
 
var d = today.getDate();
 
var h = today.getHours();
 
var min = today.getMinutes();
 
var s = today.getSeconds();
 
var milli = today.getMilliseconds();
 
//ps:用于解决宽度显示问题
 
//pps:不知为何，字符串拼接有问题，我不得不用这种神经病一样的方案来控制宽度= =||
 
if (milli >= 100) {
 
milli = (milli - (milli % 10)) / 10;
 
}
 
if (m >= 10) {
 
if (d >= 10) {
 
if (h >= 10) {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
} else {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp0" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp0" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp0" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-" + d + "&nbsp0" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
}
 
} else {
 
if (h >= 10) {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
} else {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp0" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp0" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp0" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = m + "-0" + d + "&nbsp0" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
}
 
}
 
 
 
} else {
 
if (d >= 10) {
 
if (h >= 10) {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
} else {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp0" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp0" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp0" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-" + d + "&nbsp0" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
}
 
} else {
 
if (h >= 10) {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
} else {
 
if (min >= 10) {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp0" + h + ":" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp0" + h + ":" + min + ":0" + s + "." + milli;
 
}
 
} else {
 
if (s >= 10) {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp0" + h + ":0" + min + ":" + s + "." + milli;
 
} else {
 
document.getElementById("DateAndTime").innerHTML = "0" + m + "-0" + d + "&nbsp0" + h + ":0" + min + ":0" + s + "." + milli;
 
}
 
}
 
}
 
}
 
}
 
setTimeout('getDate()', 10);
 
}
 
 
 
function getTime() {
 
var today = new Date();
 
 
 
var h = today.getHours();
 
var min = today.getMinutes();
 
 
 
if (h >= 10) {
 
if (min >= 10) {
 
document.getElementById("time").innerHTML = h + ":" + min;
 
} else {
 
document.getElementById("time").innerHTML = h + ":0" + min;
 
}
 
} else {
 
if (min >= 10) {
 
document.getElementById("time").innerHTML = "0" + h + ":" + min;
 
} else {
 
document.getElementById("time").innerHTML = "0" + h + ":0" + min;
 
}
 
}
 
setTimeout('getTime()', 1000);
 
}
 
</script>
 
<style>
 
#BGI {
 
width: 1080px;
 
height: 2340px;
 
background-image: url(BGI_TigerDAHE.jpg);
 
position: absolute;
 
left: 0px;
 
top: 0px;
 
}
 
 
 
p {
 
font-size: 60px;
 
color: white;
 
position: center;
 
margin-top: 10px;
 
}
 
 
 
#display {
 
width: 540px;
 
height: 100px;
 
position: absolute;
 
left: 300px;
 
top: 718px;
 
}
 
 
 
#time {
 
font-size: 32px;
 
position: absolute;
 
left: 65px;
 
top: 23px;
 
}
 
 
 
input {
 
outline-style: none;
 
border: 0px;
 
font-size: 40px;
 
color: #828282;
 
background-color: transparent;
 
}
 
 
 
#info1 {
 
position: absolute;
 
left: 133px;
 
top: 174px;
 
}
 
 
 
#info2 {
 
position: absolute;
 
left: 133px;
 
top: 272px;
 
}
 
 
 
#info3 {
 
position: absolute;
 
left: 133px;
 
top: 469px;
 
}
 
#info4 {
 
position: absolute;
 
left: 133px;
 
top: 370px;
 
}
 
</style>
 
</head>
 
 
 
<body onLoad="getDate();getTime()">
 
<div id="BGI">
 
<image src="http://pan.ananas.mooc.whu.edu.cn/preview/showpreview_693881268741558272.html?v=1643363924000&_from=pcuserpan">
 
<div id="display">
 
<p id="DateAndTime"></p>
 
<div id="info1">
 
<input type="text">
 
</div>
 
<div id="info2">
 
<input type="text">
 
</div>
 
<div id="info3">
 
<input type="text">
 
</div>
 
<div id="info4">
 
<input type="text">
 
</div>
 
</div>
 
</div>
 
<div id="time"></div>
 
 
 
</body>
 
 
 
</html>
