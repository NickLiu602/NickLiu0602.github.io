<template>
  <div class="bottom-container">
    <div class="box-classA">
      <div class="box-class1">
        <h4>Unmatched Services. Unmatched Excellence.</h4>
      </div>
      <div class="box-class">
        <div class="icon"><i class="fa-solid fa-poo"></i></div>
        <h4>Jarvan IV</h4>
        <p>Today is a good day to die</p>
      </div>
      <div class="box-class">
        <div class="icon"><i class=" fa-solid fa-user-secret"></i></div>
        <h4>Yasuo</h4>
        <p>Death is like the wind; always by my side.</p>
      </div>
      <div class="box-class">
      <div class="icon"><i class="fa-solid fa-user-nurse"></i></div>
      <h4>Ashe</h4>
      <p>Smart choice!</p>
    </div>
    <div class="box-class">
      <div class="icon"><i class="fa-solid fa-person-dress-burst"></i></div>
      <h4>Ezreal</h4>
      <p>Time for a true display of skill!</p>
    </div>
    <div class="box-class">
      <div class="icon"><i class="fa-solid fa-person-drowning"></i></div>
      <h4>Garen</h4>
      <p>To the Fields of  Justice!</p>
    </div>
    </div>
    
   
  </div>
</template>
<style>
.bottom-container {
  height: auto;
  width: auto;
  background-color: rgb(24, 42, 89);
  display: flex;
  flex-wrap:wrap;
  justify-content:center;
 
  
}
.bottom-container .box-classA{
  display: flex;
 flex-wrap: wrap;
 padding-top :55px;
 justify-content: center;
 margin-bottom :50px;
}
.bottom-container .box-classA .box-class1{
  margin: 20px ;
  padding: 10px;
  width: 350px;
  height: 150px;
  display: flex;
  flex-direction: row;
}
.bottom-container .box-classA .box-class{
  margin: 20px ;
  padding: 10px;
  width: 350px;
  height: 150px;
  position: relative;
  border: 2px solid rgb(15, 18, 48);
  display: flex;
  flex-direction: column;
  transition: .5s;
}
.bottom-container .box-classA .box-class:hover p,
.bottom-container .box-classA .box-class:hover h4,
.bottom-container .box-classA .box-class:hover {
  transform: scale(1.1);
   /* ------border漸層 */
  -moz-border-image: -moz-linear-gradient(top left, #3acfd5 0%, #3a4ed5 100%);
	-webkit-border-image: -webkit-linear-gradient(top left, #3acfd5 0%, #3a4ed5 100%);
	border-image: linear-gradient(to bottom right, #3acfd5 0%, #3a4ed5 100%);
	border-image-slice: 1;
  color: white;
  /* ------border漸層 */
}
.bottom-container .box-classA .box-class h4{
  color:rgb(15, 18, 48);
  padding: 10px;
}
.bottom-container .box-classA .box-class p{
  color:rgb(15, 18, 48);
  padding: 10px;
}
.bottom-container .box-classA .box-class1 h4{
  width: 80px;
  color: white;

}
.icon{
  position: relative;
  font-size: 80px;
  top: -70px;
  margin-bottom:-80px
}
@media screen and (max-width:768px){
  .bottom-container{
    
    max-height: 400px;
    overflow-y: overlay;
    display: block;
  }
  .bottom-container .box-classA .box-class p,
.bottom-container .box-classA .box-class h4,
.bottom-container .box-classA .box-class {
  transform: scale(1.1);
   /* ------border漸層 */
  -moz-border-image: -moz-linear-gradient(top left, #3acfd5 0%, #3a4ed5 100%);
	-webkit-border-image: -webkit-linear-gradient(top left, #3acfd5 0%, #3a4ed5 100%);
	border-image: linear-gradient(to bottom right, #3acfd5 0%, #3a4ed5 100%);
	border-image-slice: 1;
  color: white;
  /* ------border漸層 */
}
.bottom-container .box-classA{
  padding-top: 30px;
}
.icon{
  
  /* top: -50px;
  margin-bottom:-80px */
}
.bottom-container .box-classA .box-class{
  margin: 50px;
}
}
</style>