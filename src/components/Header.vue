<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <input type="checkbox" name="" id="menu_control">
  <div class="main-header">
    <!-- <img src="https://picsum.photos/300/300?random=1"> -->
    <div class="container">
      <a href="#" class="logo">
        <img src="../assets/logo.png" alt="vue Logo" />
      </a>
      <form class="header-search">
        <input type="_search" />
        <button><i class="fa-solid fa-magnifying-glass"></i></button>
      </form>
      <label for="menu_control" class="menu_btn">
        <span>選單</span>
      </label>
      <nav>
        <a href="#" >Home</a>
        <a href="#" >About</a>
        <a href="#" >Service</a>
        <a href="#" >Application</a>
        <a href="#" >News</a>
        <a href="#" class="no-5" >Connection</a>
      </nav>
    </div>
    <div class="header-top">
      <nav class="main-nav">
        <a href="https://www.google.com/">Home</a>
        <a href="">About</a>
        <a href="">Service</a>
        <a href="">Application</a>
        <a href="">News</a>
        <a href="">Connection</a>
      </nav>
    </div>
    <div class="header-title">
      <p>SHIPS ANYTHING</p>
      <h2>AROUND THE WORLD</h2>
      <a href="">GO</a>
    </div>
    <div class="header-bottom">
      <div class="item">
        <a href="" class="icon-class">
          <div class="icon"><i class="fa-solid fa-truck-fast"></i></div>
          <h3>CAR</h3>
          <p>BigTruck</p>
        </a>
      </div>
      <div class="item">
        <a href="" class="icon-class">
          <div class="icon"><i class="fa-solid fa-hippo"></i></div>
          <h3>ANIMAL</h3>
          <p>Hippo</p>
        </a>
      </div>
      <div class="item">
        <a href="" class="icon-class">
          <div class="icon"><i class="fa-solid fa-cart-plus"></i></div>
          <h3>SHOPPING</h3>
          <p>ShoppingCart</p>
        </a>
      </div>
      <div class="item">
        <a href="" class="icon-class">
          <div class="icon"><i class="fa-solid fa-plane"></i></div>
          <h3>TRANSPORT</h3>
          <p>Air Plane</p>
        </a>
      </div>
      <div class="item">
        <a href="" class="icon-class">
          <div class="icon"><i class="fa-solid fa-poo-storm"></i></div>
          <h3>WEATHER</h3>
          <p>Storm</p>
        </a>
      </div>
    </div>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  list-style: none;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  box-sizing: border-box;
}
.menu_btn{
  display: none;
}
#menu_control{
  display: none;
}
.container nav {
  display: none;
}
.main-header {
  background-color: #ccc;
  background-image: url("../image/pexels-sevenstorm-juhaszimrus-443383.jpg");
  background-size: cover;
  height: auto;

  /* justify-content:space-around; */
}
.header-top {
  margin: auto;
  padding: 10px;
  display: flex;
  justify-content: space-between;
}
.main-header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
  max-width: 1200px;
  margin: auto;
}
.main-header .logo {
  width: 40px;
}
.main-header .logo img {
  width: 100%;
  vertical-align: middle;
}
.header-top .main-nav {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  margin: auto;
}
.header-top .main-nav a {
  cursor:pointer;
	position:relative;
	padding:10px 10px;
	background:transparent;
	font-size:28px;
	border-top-right-radius:25px;
	border-bottom-left-radius:25px;
	transition:all 1s;
  text-decoration:none;
  color: black;
}
/* -------------------------------------- */
.header-top .main-nav a:after,
.header-top .main-nav a:before {
  content: " ";
  width: 10px;
  height: 10px;
  position: absolute;
  transition: all 1s;
}
.header-top .main-nav a:after {
  top: 0px;
  left: 0px;
  border-top: 5px solid black;
  border-left: 5px solid black;
  
}
.header-top .main-nav a:before {
  bottom: 0px;
  right: 0px;
  border-bottom: 5px solid black;
  border-right: 5px solid black;
}
.header-top .main-nav a:hover {
  border-top-right-radius: 0px;
  border-bottom-left-radius: 0px;
  background-color: #fff;
}
.header-top .main-nav a:hover:before,
.header-top .main-nav a:hover:after {
  width: 95%;
  height: 90%;
}

/* --------------------------------------- */
.main-header .header-search {
  display: flex;
}
.main-header .header-search button,
.main-header .header-search input {
  border: none;
  background-color: #fff;
  padding: 8px;
}
.main-header .header-search button:hover {
  transform: scale(1.1);
}
.main-header .header-search button:focus,
.main-header .header-search input:focus {
  outline: none;
}
.main-header .header-search button {
  border-radius: 0 200px 200px 0;
}
.main-header .header-search input {
  border-radius: 200px 0 0 200px;
}
.main-header .header-title {
  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
}
.main-header .header-title p {
  margin-top: 20px;
  padding: 5px;
}
.main-header .header-title a {
  margin-top: 15px;
  width: 40px;
  /* align-items:center; */
  background-color: white;
  text-decoration: none;
  padding: 1px 10px;
  border-radius: 100px;
  font-size: 13px;
  transform: translateY(0);
  transition: 0.5s;
}
.main-header .header-title a:hover {
  transform: translateY(-5px);
}
.header-bottom {
  margin-top: 50px;
  height:98px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}
.header-bottom .item {
  padding: 10px;
  width: 140px;
  height: 140px;
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  transform: translateY(0);
  transition: 1s,border-radius 1s,margin 1s;
}
.header-bottom .item:hover {
  background-color: rgb(2, 85, 108);
  transform: translateY(-5px) scale(1.2);
  color: #fff;
  border-radius: 100px;
  margin:0 2%
}
.header-bottom .item .icon {
  font-size: 55px;
  opacity: 0.9;
  color: #ccc;
}
.header-bottom .item:hover h3,
.header-bottom .item:hover p,
.header-bottom .item:hover .icon {
  color: #fff;
}
.header-bottom .item .icon-class {
  margin-top: 85px;
  text-decoration: none;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.header-bottom .item h3 {
  padding: 5px;
  color: rgb(4, 4, 144);
  font-size: 14px;
}
.header-bottom .item p {
  color: #ccc;
  font-size: 10px;
}
@media screen and (max-width:768px) {
  .main-header .header-search {
    display: none;
  }
  .header-top{
    display: none;
  }
  .main-header{
    height:300px;
    display: flex;
    flex-direction: column;
  }
  .menu_btn{
    width: 50px;
    height: 50px;
    background-color:rgb(41, 132, 229);
    display: block;
    position: absolute;
    top: 5px;
    right: 5px;
    border-radius:20%;
  }
  /* .menu_btn:hover{
    opacity:1;
    transform: scale(1.1);
  } */
  .menu_btn span{
    opacity: 0;
  }
  .menu_btn::before{
  content: '';
  position: absolute;
  height: 5px;
  width: 40px;
  left: 5px;
  background-color:white;
  border-radius:10%;
  top: 0;
  bottom: 0;
  margin: auto;
  box-shadow: 0px 12px 0px white,
  0px -12px 0px white;
  }
  #menu_control{
    position:absolute;
  z-index: -2;
  opacity: 0;
  }
   
  
  .container nav{
  width: 40%;
  height:calc(100vh - 295px);
  background-color: black;
  position: absolute;
  top: 60px;
  left:-100%;
  transition: .6s;
  
  display: block;
  z-index: 5;
  border-radius:20px;
}
.container nav a{ 
  display: block;
  text-decoration: none;
  color:rgb(41, 132, 229);
  padding: 27px 20px;
  border-bottom: 2px solid rgb(41, 132, 229);
  font-weight:900;
  font-family:Verdana, Geneva, Tahoma, sans-serif;
 
}
.container .no-5{
  border-bottom:none
}
/* .container nav:hover,
.container nav a:hover{
  opacity:1;
} */
#menu_control:checked ~ .main-header nav{
 left:0px;
}

.header-bottom .item .icon{
  font-size: 38px;
}
.header-bottom .item .icon-class{
  margin-top: 70px;
}
.middle-title h2{
  display: flex;
  justify-content: center;
  height: auto;
}
.header-bottom .item {
  background-color: rgb(2, 85, 108);
  width: 100px;
  height:auto;
  color: #fff;
  border-radius: 100px;
  margin:0 1%;
  transform: scale(1);
  transition: .1s;
}.header-bottom .item:hover{
  transform: scale(1);
  margin:0 1%
}
.header-bottom .item h3,
.header-bottom .item p,
.header-bottom .item .icon {
  color: #fff;
}
}
@media screen and (max-width:320px) {
  .container nav{
    width: 100%;
  }
}
@media screen and (max-width:560px) {
  
  .header-bottom{
    max-width:100%;
    overflow: overlay;
    display: flex;
    flex-direction: column;
    justify-content: unset;
    margin-top: 18px;
  }
  .main-header{
   min-width:100% ;
  }
}
@media screen and (max-width:410px) {
  .main-header{
    height: auto;
  }
}
</style>