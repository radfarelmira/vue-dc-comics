<template>
  <div id="app">
    <Header/>

    <main>
    <SeriesList/>

    <SubMain/>
    </main>
    

    <Footer/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SeriesList from "./components/SeriesList.vue";
import SubMain from "./components/SubMain.vue";
import Footer from "./components/Footer.vue";



export default {
  name: "App",
  components: {
    Header,
    Footer,
    SubMain,
    SeriesList,
  },
};
</script>

<style lang="scss">
@import './style/general.scss';
@import './style/common.scss';
@import './style/variables.scss';


</style>
