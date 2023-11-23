
<template>
    <Banner/>
  <div class="main-c"> 
    <h1>
      MONTE SEU LANCHE 
    </h1>
    <BurgerForm/>
  </div>
</template>

<script>

import Banner from '../components/Banner.vue';
import BurgerForm from '../components/BurgerForm.vue';


export default{
  components:{
    Banner,
    BurgerForm,
   
},
  name:"Home",
}

</script>