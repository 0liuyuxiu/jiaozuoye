<!DOCTYPE html>
<html>
<head>
<title>xiuye</title>
<meta charset="utf-8"/>
<style>
#id{width:1800px;height:400px;position:relative; top:60px;left:50px;overflow:hidden;}
img{width:1800px;height:400px;}
li{float:left;list-style:none;}
#sw{position:relative;display:inline-block;z-index:4;width:18000px;height:400px;}
#xiu{position:absolute;z-index:10; top:420px;left:850px;}
#xiu li{display:inline; font:left; width:20PX; height:20px; border-radius:50%;background:white;margin-left:20px;}
</style>
<script>
window.onload=function(){
var oDiv=document.getElementById('de');
var oK=document.getElementById('sw');
var oImg=document.getElementsByTagName('img');
var oUl=document.getElementById('xiu');
var aLi=oUl.getElementsByTagName('li');
var aLi1=document.getElementById('1');
var aLi2=document.getElementById('2');
var aLi3=document.getElementById('3');
var aLi4=document.getElementById('4');
var xiuzi=document.getElementById('xiu2');
var oNi=document.getElementById('ni');
var oWo=document.getElementById('wo');
var c=-1800;
var d=1;
var i=0;
var liu;
var e=setInterval(function(){
	aLi[i].style.background="red";
	for(var w=0;w<4;w++){
		if(w!=i){
			aLi[w].style.background="white";
		}
	}
	i=(i+1)%4;
	
	var y=setInterval(
		function(){
		if(oK.offsetLeft<c){
			clearInterval(y);
			c-=1800;
		}
		else{
		oK.style.left=oK.offsetLeft-5+"px";}
		if(oK.offsetLeft<-oK.offsetWidth/2){
		oK.style.left=0;c=-1800;
			}	
	},2);
	
},3000);
oNi.onclick=function(){
	oK.style.left=oK.offsetLeft-1800+"px";
    i++;
	if(oK.offsetLeft<-7200)
		oK.style.left=0+"px";
	
	clearTimeout(e);
	liu=setInterval(function(){
    if(oK.offsetLeft==-1800)
    	i=1;
	aLi[i].style.background="red";
	for(var w=0;w<4;w++){
		if(w!=i){
			aLi[w].style.background="white";
		}
	}
	i=(i+1)%4;
	
	var y=setInterval(
		function(){
		if(oK.offsetLeft<c){
			clearInterval(y);
			c-=1800;
		}
		else{
		oK.style.left=oK.offsetLeft-3+"px";}
		if(oK.offsetLeft<-oK.offsetWidth/2){
		oK.style.left=0;c=-1800;
			}	
	},2);
	
},3000);
}
oWo.onclick=function(){
	oK.style.left=oK.offsetLeft+1800+"px";
    i++;
	if(oK.offsetLeft<-7200)
		oK.style.left=0+"px";
	clearInterval(liu);
	clearInterval(e);
	setInterval(function(){
    if(oK.offsetLeft==-1800)
    	i=1;
	aLi[i].style.background="red";
	for(var w=0;w<4;w++){
		if(w!=i){
			aLi[w].style.background="white";
		}
	}
	i=(i+1)%4;
	
	var y=setInterval(
		function(){
		if(oK.offsetLeft<c){
			clearInterval(y);
			c-=1800;
		}
		else{
		oK.style.left=oK.offsetLeft-3+"px";}
		if(oK.offsetLeft<-oK.offsetWidth/2){
		oK.style.left=0;c=-1800;
			}	
	},2);
	
},3000);
}
aLi1.onclick=function(){
	oK.style.left=0+"px";
    c=-1800;
    this.style.background="red";
    aLi2.style.background="white";
    aLi3.style.background="white";
    aLi4.style.background="white";
    d=0;
}
aLi2.onclick=function(){
	oK.style.left=-1800+"px";
    c=-3600;
    this.style.background="red";
    aLi1.style.background="white";
    aLi3.style.background="white";
    aLi4.style.background="white";
    d=1;
}
aLi3.onclick=function(){
	oK.style.left=-3600+"px";
    c=-5400;
    this.style.background="red";
    aLi1.style.background="white";
    aLi2.style.background="white";
    aLi4.style.background="white";
    d=2;
}
aLi4.onclick=function(){
	oK.style.left=-5400+"px";
    c=-7200;  
    this.style.background="red";
    aLi1.style.background="white";
    aLi2.style.background="white";
    aLi3.style.background="white";
    d=3;
}


setInterval(function(){
	xiuzi.style.left=xiuzi.offsetLeft-2+"px";
	if(xiuzi.offsetLeft==-300){
       xiuzi.style.left=1600+"px"
	}
},12);
}


</script>
</head>
<body >
<div style="width:200px;height:400px;margin:75px 1700px;background:white;position:fixed;z-index:5;">
</div>
<div style="width:200px;height:385px;position:fixed; z-index:6;margin:75px -50px;background:white;">
</div>
<div style="width:400px;height:30px;position:fixed;z-index:8; margin:46px 1600px; background:#ccc;">
</div>
<p  id="ni" href="javascript" style="width:100px; height:100px; position:fixed;margin:160px 130px; z-index:10;font-size:100px;">
  <
</p>
<p  id="wo" href="javascript" style="width:100px; height:100px; position:fixed;margin:160px 1640px; z-index:10;font-size:100px;">
  >
</p>
<div style="position:absolute;margin-left:-20px;margin-top:46px; height:30px; width:1700px; background:#ccc;color:red;display:block;">
<p id="xiu2" style="position:fixed; z-index:3; left:110px;top:45px;">[温馨提示]最近有不少不法分子在网上骗人，请大家注意！</p>
</div>
<div id="id">
<ul id="sw">
<li><img src="D:\360安全浏览器下载\b1.png"/></li>
<li><img src="D:\360安全浏览器下载\b2.png"/></li>
<li><img src="D:\360安全浏览器下载\b3.png"/></li>
<li><img src="D:\360安全浏览器下载\b4.png"/></li>
<li><img src="D:\360安全浏览器下载\b5.png"/></li>
<li><img src="D:\360安全浏览器下载\b1.png"/></li>
<li><img src="D:\360安全浏览器下载\b2.png"/></li>
<li><img src="D:\360安全浏览器下载\b3.png"/></li>
<li><img src="D:\360安全浏览器下载\b4.png"/></li>
<li><img src="D:\360安全浏览器下载\b5.png"/></li>
</ul>
</div>
<ul id="xiu" >
<li id="1">1</li>
<li id="2">2</li>
<li id="3">3</li>
<li id="4">4</li>
</ul>
</body>
</html>
