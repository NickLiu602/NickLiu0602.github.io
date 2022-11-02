<!-- eslint-disable vue/multi-word-component-names -->
<template>
<div class="main-footer">
  <div class="container">
    <div class="footer-item">
      <h5><i class="fa-solid fa-mountain-sun"></i></h5>
      <p>Shakespeare’s play about the doomed romance of two teenagers from feuding families is the most famous love story ever written.</p>
      <div class="icon-class">
        <a href=""><i class="fa-solid fa-house"></i></a>
        <a href=""><i class="fa-solid fa-user"></i></a>
        <a href=""><i class="fa-solid fa-download"></i></a>
        <a href=""><i class="fa-solid fa-image"></i></a>
      </div>
    </div>
    <div class="footer-item">
      <h4>Service</h4>
      <div class="item-one">
        <a href=""><i class="fa-solid fa-fish-fins"></i> Beauty</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> English</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Success</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Good luck</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Opportunity</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Amazing</a>
      </div>
    </div>
    <div class="footer-item">
      <h4>Coffee Shop</h4>
      <div class="item-one">
        <a href=""><i class="fa-solid fa-fish-fins"></i> Friendship</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Remember</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Chance</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Conversation</a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Thank you </a>
        <a href=""><i class="fa-solid fa-fish-fins"></i> Appreciate</a>
      </div>
    </div>
    <div class="footer-item footer-subscript">
      <h4>Subscription</h4>
      <form>
        <input type="text">
        <input type="submit" value="Subscript">
      </form>
      <nav>
        <a href=""></a>
      </nav>
    </div>
  </div>
  <div class="copyright">
    Copyright &copy; 2022.09.15 Bowa 程式學院
  </div>
</div>
</template>
<style>
  .main-footer{
    margin-top:5px;
    padding: 60px 0 0 0;
    background: rgb(7, 25, 70);
    width: auto;
   
  
  }
  .main-footer .container{
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }
  .footer-item{
    width: 220px;
    height: 280px;
    display: flex;
    margin: 5px 20px;
    flex-direction: column;
  }
  
  .footer-item h4{
    color: white;
    font-size: 24px;
  }
  .footer-item h5{
    font-size: 80px;
    color: white;
  }
  .footer-item p{
    color: white;
    font-size: 18px;
    padding: 30px 0 0 0 ;
  }
  .footer-item .item-one{
    display: flex;
    flex-direction: column;
    transform:translateY(0);
    transition: .3s;
  }
  .footer-item .item-one a{
    color: white;
    line-height: 1.5;
    text-decoration: none;
    padding: 5px 0;
    font-size: 18px;
    
  }
  .footer-item .item-one a:hover{
    transform: translateY(-5px);
  }
  .copyright{
    display: block;
    margin: 5px 0 0;
    top: 80px;
    text-align: center;
    width: 100%;
    color: white;
    font-size: 14px;
  }
  .footer-item .icon-class{
  
    margin-top:15px;
    transition: .5s;
    display: flex;
   
  }
  .footer-item .icon-class a{
    color: white;
    padding: 10px;
    transform:translateY(0);
  }
  .footer-item .icon-class a:hover{
    transform: translateY(-5px);
  }
  .footer-subscript form{
    display: flex;
    width: 100%;
    margin: auto 0;

  }
  .footer-subscript input[type="text"],
  .footer-subscript input[type="submit"]{
    border:none;
    padding: 5px 0;
  }
  .footer-subscript input[type="submit"]{
    color:white;
    background: rgb(6, 6, 151);
  }

  .footer-subscript{
    display: flex;
    flex-direction: column;
  }
</style>