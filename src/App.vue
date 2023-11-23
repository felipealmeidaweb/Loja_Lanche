

<template>
 
   <NavBar :logo="logoSrc" :alt="App_name"/>
   
  <RouterView />
  <Footer_z/>

</template>

<script>
import Footer_z from './components/Footer.vue';
import NavBar from './components/NavBar.vue';
export default{
  components:{
    NavBar,
    Footer_z,
},
data(){
  return{
    logoSrc:"/img/lancheIcon.png",
    App_name:"logoPng"
  }
}
}

</script>

<style>
*{
  font-family: Arial, Helvetica, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.main-c{
  margin: 50px;
  min-width: 250px;
}
h1{
  text-align: center;
  font-size: 43px;
  margin-bottom: 30px;
}
</style>
