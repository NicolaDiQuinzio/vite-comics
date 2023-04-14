<template>
      <header class="container row justify-content-between align-items-center  h-100 mx-auto">
        <div class="col-2 p-3">
            <img class="img-fluid" src="../assets/img/dc-logo.png" alt="dc-logo">
        </div>
        <div class="h-100 col-10 d-flex justify-content-end ">
            <ul class="d-flex justify-content-center gap-3 flex-wrap h-100 m-0 p-0 list-unstyled">
               <li v-for="(link,index) in menù" :key="index">
                <span class=" nav-link"><a :href="link.url" class="text-decoration-none text-black ">  {{ link.text }}</a></span>
               </li>
            </ul>
        </div>
    </header>

</template>

<script>
import headerMenù from '../file-js/file';
export default{
    data(){
        return{
            menù: headerMenù
        }
    }
}
</script>

<style lang="scss" scoped>
span{
    padding-bottom: 20px;
}
.nav-link:hover {
border-bottom: 3px solid #3291ef;
}
</style>