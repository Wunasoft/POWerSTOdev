<script lang="ts">
	import {RouterLink} from 'vue-router'
	
	export default {
		name: "HeaderLogo",
	};
</script>

<template>
<div class="logoline">
	<div class="logo">
		<a href="./index.html" target="_self">
		<img class="logoimg" src="../../assets/images/logo.png"/>
		</a>
	</div>
	<div class="logomenu">
		<!-- <a id="menulink" href="./investment.html" >투자하기</a>
		<a id="menulink" href="./aboutus.html" >ABOUT US</a>
		<a id="menulink" href="./notice.html" >공지사항</a>
		<a id="menulink" href="./login.html" >로그인</a> -->
		<RouterLink to="/investment">투자하기</RouterLink>
    <RouterLink to="/aboutus">ABOUT US</RouterLink>
    <RouterLink to="/notice">공지사항</RouterLink>
    <RouterLink to="/login">로그인</RouterLink>
	</div>
</div>
</template>


<style >
.logoline{
	width:100%; height:3.6em;
	display:flex;
	margin:0em;
	margin-top:0.3em;
    }
.logo{
float:left;
}
.logoimg{
	width:124px;
	padding-left : 0.9em;
}
.logomenu{
	text-decoration:none;
	width:100%;
	line-height:50px;
	vertical-align:bottom; 
	text-align:center;
}
#menulink{
	text-decoration-line:none;
	font-size:.95em;
	font-weight:bold;
	font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	text-decoration-color:deepskyblue;
	margin:0 1.2em; 
    }
</style>


