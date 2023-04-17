<template>
    <div class="d-flex flex-wrap justify-content-center">
        <Cardprops v-for="(items) in cards" :image="items.thumb" :title="items.series"/>
    </div>
</template>


<script>
import { Dccard } from '../file-js/file';
import Cardprops from './Cardprops.vue';
export default{
    name: 'Cardcomponent',
     props: ['image', 'title'],
    components:{
    Cardprops,
   },
    data(){
        return{
            cards: Dccard,
            
        }
    }
}
</script>
<style lang="scss" scoped>

</style>