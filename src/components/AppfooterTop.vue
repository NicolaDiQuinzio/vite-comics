<template>
<div class="bg-img position-relative overflow-hidden">
<div class="container  ">
    <div class="row ">
        <div class="col pt-5">
            <h5 class="text-white"> DC Comics</h5>
            <ul class="list-unstyled">
                <li v-for="(link,index) in Dccomics" :key="index" class="g-color">
                {{ link.text }}
               </li>
            </ul>
            <h5 class="text-white"> Shop</h5>
            <ul class="list-unstyled pb-5">
                <li v-for="(link,index) in Shop" :key="index" class="g-color">
                {{ link.text }}
               </li>
            </ul>
        </div>
        <div class="col pt-5">
            <h5 class="text-white"> DC</h5>
            <ul class="list-unstyled">
                <li v-for="(link,index) in Dc" :key="index" class="g-color">
                {{ link.text }}
               </li>
            </ul>
        </div>
        <div class="col pt-5">
            <h5 class="text-white"> Sites</h5>
            <ul class="list-unstyled">
                <li v-for="(link,index) in Sites" :key="index" class="g-color">
                {{ link.text }}
               </li>
            </ul>
        </div>
        <div class="col">
                <img class="img-fluid logo-bg" src="../assets/img/dc-logo-bg.png" alt="Logo Dc">
        </div>
            

    </div>
</div>
</div>
</template>
<script>
import  {DCcomicsMenù, ShopMenù, DcMenù, SitesMenù} from '../file-js/file'
export default{
    data(){
        return{
            Dccomics: DCcomicsMenù,
            Shop: ShopMenù,
            Dc: DcMenù,
            Sites:SitesMenù,
        }
    }
}
</script>

<style lang="scss" scoped>

.bg-img{
    background-image: url(../assets/img/footer-bg.jpg);
}
.g-color{
    color: #959595 ;
}

.logo-bg{
    max-width: 470px;
    position: absolute;
    right: 0;
    top: -5%;
}

</style>

