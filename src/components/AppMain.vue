<template>
  
 <section >
    <div class="jumbotron h-jumbotron position-relative ">
        <div>
                <button class="text-white bg-primary btn btn-jumbo ">CURRENT SERIES</button>
        </div>
    </div>  
</section>
<section>
    <CardsComponent/>
</section>

  
</template>

<script>

import Cardprops from './Cardprops.vue';
import CardsComponent from './CardsComponent.vue';
import CardsComponent from './CardsComponent.vue';


    export default{
    Cardprops,
    CardsComponent,
    components: { CardsComponent }
}


</script>

<style lang="scss" scoped>
.h-jumbotron{
    background-image: url(../assets/img/jumbotron.jpg);
    height: 300px;
   background-size: cover;
}
.btn-jumbo{
    position: absolute;
    bottom: -5%;
    left:20%
}



</style>