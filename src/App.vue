<template>
  <Header></Header>
  <Body></Body>
  
    <BodyMiddle></BodyMiddle>

  <div id="App2" v-if="isOpen1">
    <BodyBottom></BodyBottom>
  </div>
  <div id="App3" v-if="isOpen2">
    <Footer></Footer>
  </div>
</template>

 <script>
import Header from "./components/Header.vue";
import Body from "./components/Body.vue";
import BodyMiddle from "./components/BodyMiddle.vue";
import BodyBottom from "./components/BodyBottom.vue";
import Footer from "./components/Footer.vue";
import { onMounted, onUnmounted ,ref} from "vue";
export default {
  components: {
    Header,
    Body,
    BodyMiddle,
    BodyBottom,
    Footer,
  },
  setup() {
    const isOpen1 = ref(false);
    const isOpen2 = ref(false);
    
    let index= 0;
    function scrollHandle() {
     
      let scrollHeight = document.body.scrollHeight;
      let scrollTop =
        document.body.scrollTop || document.documentElement.scrollTop;
      let clientHeight = document.documentElement.clientHeight;

      let distance = scrollHeight - scrollTop - clientHeight;
      
      if ( distance < 60) {
        index++;
        if(index===1){
          isOpen1.value = true;
        }
        if(index===2){
          isOpen2.value = true;
        }
       
      }
      
      
     
      console.log(index);
      console.log(distance);
    }
    onMounted(() => {
      window.addEventListener("scroll", scrollHandle, false);
     
      
    });
    onUnmounted(() => {
      window.removeEventListener("scroll", scrollHandle, false);
    });
    return {
      isOpen1,
      isOpen2,
     
    }
  },
 
};
</script>
 
 <style>
</style>
