<template>
  <a href="https://css-tricks.com/aos-css-driven-scroll-animation-library/"></a>
  <a href="https://github.com/michalsnik/aos"></a>
  <a href="https://michalsnik.github.io/aos/"></a>
  <div class="bodyMiddle">
    <div class="container-bottom">
      <div class="box left">
        <h3>Freight Company With a Difference. Innovation.</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque nec
          turpis consequat, pulvinar nibh ut, tempus enim. Donec dignissim
          scelerisque eros, non scelerisque neque. Nam id ipsum pellentesque,
          vulputate turpis.
        </p>
        <div class="bottom">
          <h5>Good Day</h5>
          <p>keep learning</p>
        </div>
      </div>
      <div class="box middle">
        <div class="title">
          <img src="https://picsum.photos/245/130?random=4" />
        </div>
        <div class="middle">
          <h5>How Are You Today?</h5>
          <p>
            Praesent lectus diam, ultricies nec bibendum vitae, facilisis non
            purus. Cras neque ex, hendrerit volutpat nisl vel, facilisis posuere
            tellus. Nulla imperdiet rhoncus dolor, eu aliquam nisl.
          </p>
        </div>
        <a href="" class="button">
          <p>></p>
        </a>
      </div>
      <div class="box right">
        <div class="title">
          <img src="https://picsum.photos/245/130?random=5" />
        </div>
        <div class="middle">
          <h5>It Is A Good Day</h5>
          <p>
            Donec porta odio et erat vulputate porttitor. Maecenas rutrum risus
            dignissim, rhoncus purus vel, vehicula tellus. Fusce scelerisque
            augue odio, vitae imperdiet metus suscipit sit amet.
          </p>
        </div>
        <a href="" class="button">
          <p>></p>
        </a>
      </div>
    </div>
  </div>
</template>

<style>
.container-bottom {
  display: flex;
  justify-content: center;
  background-color: #ccc;
  flex-wrap: wrap;
  box-sizing: border-box;
}
.box {
  margin:0;
  width: 250px;
  height: 350px;
  padding: 10px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}
.container-bottom .box h3 {
  padding: 10px;
  color: rgb(6, 6, 98);
  width: 250px;
}
.container-bottom .box p {
  padding: 5px;
  font-size: 14px;
}
.container-bottom .box .bottom {
  padding-top: 20px;
}
.container-bottom .box .bottom h5 {
  color: rgb(6, 6, 98);
}
.container-bottom .box .middle h5 {
  color: rgb(6, 6, 98);
  padding: 5px;
}
.container-bottom .box .button {
  text-decoration: none;
  width: 40px;
  height: 40px;
  text-align: center;
  background-color: white;
  border-radius: 100px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  transition: 0.5s;
  transform: scale(1);
}
.container-bottom .box img {
  width: 240px;
  height: 140px;
  padding: 5px;
}
.container-bottom .box .button:hover {
  background-color: rgb(65, 155, 239);
  transform: scale(1.2);
}
.container-bottom .box .button:hover p {
  color: white;
}
.container-bottom .box .button p {
  font-size: 20px;
  color: rgb(65, 155, 239);
}
@media screen and (max-width: 768px) {
  .container-bottom{
    display: block;
    max-height: 350px;
    width: auto;
    overflow-y: overlay;
   
  }
  .box.middle,
  .box.right{
    width: auto;
    flex-direction: row;
    align-items:center ;
  }
  .box.middle img,
  .box.right img{
    width: 360px;
    height: 240px;
    border-radius: 20px;
  }
  .box.middle .middle{
    padding:0 20px;
  }
  .box.middle .button ,
  .box.right .button {
  margin-top: 40%;
  padding: 20px;
  }
  .box.middle .button p,
  .box.right .button p{
    margin-left:-10px ;
  }
  .box.left{
  display: flex;
  width: auto;
  }
  .box.left p,
  .box.middle p,
  .box.right p{
    font-size: 24px;
  }
  .container-bottom .box img{
    
  }
}
@media screen and (max-width: 630px) {
  /* .box.middle img,.box.right img{
    width: 300px;
    height: 200px;
  } */
  .box.middle,.box.right,.box.left{
    display: flex;
    flex-direction: column;
    height: auto;
  }
  .container-bottom .box .button{
    margin-top:0px;
  }
}
@media screen and (max-width: 320px) {
   .box.middle img,.box.right img{
    width: 300px;
    height: 200px;
  }
}
</style>