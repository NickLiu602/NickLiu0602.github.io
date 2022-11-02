<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="container">
    <div class="middle-title">
      <h2>Why Choose Us?</h2>
      <p></p>
    </div>
    <div class="middle-body">
      <div class="img-class">
        <div class="img1">
          <img src="https://picsum.photos/200/200?random=1" />
        </div>
        <div class="img2">
          <img src="https://picsum.photos/200/200?random=2" />
        </div>
        <div class="img3">
          <img src="https://picsum.photos/200/200?random=3" />
        </div>
      </div>
      <div class="content-class">
        <div class="content1">
          Pellentesque molestie tincidunt sem, nec tempus nibh volutpat in.
          Etiam vehicula felis congue, sagittis mauris ut, posuere ligula. Etiam
          sodales, orci et suscipit gravida, ante ante elementum dui, vitae
          sollicitudin felis justo volutpat quam.
          Pellentesque molestie tincidunt sem, nec tempus nibh volutpat in.
          Etiam vehicula felis congue, sagittis mauris ut, posuere ligula. Etiam
         
        </div>
        <div class="content2">
          at viverra purus nunc at leo. Nulla euismod imperdiet massa id
          lobortis. Vivamus tristique massa vitae ligula sagittis, sit amet
          pulvinar massa malesuada. Vivamus id risus orci. In elit quam, dictum
          fermentum ex elementum, dapibus pulvinar urna. at viverra purus nunc at leo. Nulla euismod imperdiet massa id
          lobortis. Vivamus tristique massa vitae ligula sagittis, sit amet
         \
        </div>
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
}
.container {
}
.container .middle-title h2 {
  text-align: center;
  margin-top: 50px;
 
  color: rgb(6, 6, 166);
}
.middle-body {
  display: flex;
  height: auto;
  padding: 0 40px;
  margin: auto;
  justify-content: space-around;
}
.middle-body .img-class {
  width: 400px;
  height: 500px;
  display: flex;
  justify-content: center;
}
.middle-body .img-class .img1 {
  position: relative;
  top: 55px;
  left: 80px;
  width: 300px;
  height: 300px;
  transform: translateY(0) translateX(0);
  transition: 0.5s;
  border-radius: 75px;
}
.middle-body .img-class img {
  border-radius: 75px;
  width: 300px;
  height: 300px;
}
.middle-body .img-class .img1:hover {
  transform: translateY(-20px) translateX(20px) scale(1.1);
  box-shadow: 1px 10px 120px rgb(194, 64, 64);
  z-index: 5;
}
.middle-body .img-class .img2 {
  left: -200px;
  top: 110px;
  width: 300px;
  height: 300px;
  position: relative;
  transform: translateY(0) translateX(0);
  transition: 0.5s;
  border-radius: 75px;
}
.middle-body .img-class .img2:hover {
  box-shadow: 1px 10px 120px rgb(52, 235, 110);
  transform: translateY(-20px) translateX(0) scale(1.1);
  z-index: 5;
}
.middle-body .img-class .img3 {
  position: absolute;
  width: 300px;
  height: 300px;
  margin: 80px;
  transform: translateY(0) translateX(0);
  transition: 0.5s;
  border-radius: 75px;
}
.middle-body .img-class .img3:hover {
  box-shadow: 1px 10px 80px rgb(129, 129, 242);
  transform: translateY(20px) translateX(20px) scale(1.1);
  z-index: 5;
}
.middle-body .content-class {
  width: auto;
  height: auto;
  white-space: pre-wrap;
  display: flex;
  flex-direction: column;
  margin: auto;
}
.middle-body .content-class .content1 {
  width: 100%;

  padding: 5px;
  font-size: 20px;
  padding: 10px;
  margin: 10px;
  display: flex;
}
.middle-body .content-class .content2 {
  padding: 5px;
  margin-top: 6%;
  font-size: 20px;
  padding: 10px;
  margin: 10px;
  width: 100%;

  display: flex;
}
@media screen and (max-width: 768px) {
  .middle-body {
   
    padding: 0;
    margin: 0;
    flex-direction: column;
  }
  .middle-body .img-class {
    justify-content: center;
    
  }
  .middle-body .img-class .img1 {
    width: 200px;
    height: 200px;
    position: unset;
    margin: 5px;
  }
  .middle-body .img-class .img2 {
    position: unset;
    width: 200px;
    height: 200px;
    margin: 5px;
  }
  .middle-body .img-class .img3 {
    position: unset;
    width: 200px;
    height: 200px;
    margin: 0;
    margin: 5px;
  }
  .middle-body .img-class img {
    width: auto;
    height: auto;
  }
  .middle-body .img-class {
    align-items: center;
    width: auto;
    height: auto;
    display: flex;
  }
  .middle-body .content-class .content2 {
    margin-top: 0;
  }
  .container .middle-title h2 {
    padding-top:0px;
    margin: 50px 0 20px;
  }
}
@media screen and (max-width: 630px) {
  .middle-body .img-class{
    flex-wrap: wrap;
  
  }
  .content-class{
    justify-content: space-around;
    margin: 0;
  }
  .middle-body{
    display: flex;
    flex-direction: row;
  }
}
@media screen and (max-width: 320px) {
  .middle-body{
    display: flex;
    flex-direction: column;
  
  }
}
</style>