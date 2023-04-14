<template>

<Appheader/>
<AppBlueSection/>
<AppfooterTop/>
<Appfooter/>>

</template>
<script>


import Appheader from './components/Appheader.vue';
import AppBlueSection from './components/AppMain.vue'
import AppfooterTop from './components/AppfooterTop.vue'
import Appfooter from './components/Appfooter.vue';


export default{
    name: "App",
    components: Appheader,
    components: AppBlueSection,
    components :AppfooterTop,
    components:Appfooter,
    components: { Appheader, AppBlueSection, AppfooterTop, Appfooter }
}</script>

<style lang="css" scoped></style>