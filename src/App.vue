<template>

<Appheader/>
<main>

<AppMain/>
<CardsComponent/>
<BlueSection/>
<AppfooterTop/>
</main>
<Appfooter/>>

</template>
<script>


import Appheader from './components/Appheader.vue';
import AppMain from './components/AppMain.vue'
import Cardprops from './components/Cardprops.vue';
import CardsComponent from './components/CardsComponent.vue';
import BlueSection from './components/BlueSection.vue';
import AppfooterTop from './components/AppfooterTop.vue'
import Appfooter from './components/Appfooter.vue';


export default{
    name: "App",
    components: Appheader,
    components: AppMain,
    components:Cardprops,
    components:CardsComponent,
    components:BlueSection,
    components :AppfooterTop,
    components:Appfooter,
    components: { Appheader, AppMain, Cardprops,CardsComponent,BlueSection, AppfooterTop, Appfooter }
}</script>

<style lang="css" scoped>
</style>