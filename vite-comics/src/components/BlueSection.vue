<template>
    <section class="bg-primary pt-3 pb-3">
        <div class="container">
            <div class="h-100 col-10 d-flex justify-content-end ">
            <ul class="d-flex justify-content-center gap-3 flex-wrap  m-0 p-0 list-unstyled ">
               <li v-for="(link,index) in Bluecard" :key="index" class=" text-decoration-none text-white ">
                 {{ link.img }}
               </li>
            </ul>
        </div>
        </div>
    </section>
</template>


<script>
import { Blueicons } from '../file-js/file';
export default{
   name: 'BlueSection',
   data(){
       return{
        Bluecard: [...Blueicons]
           
       }
   }
}

</script>

<style lang="scss" scoped>
.cardblue{
    width: 50px;
    height: 38px;
   
}
</style>