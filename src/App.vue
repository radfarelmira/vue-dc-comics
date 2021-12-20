<template>
  <div id="app">
    <Header/>

    <main>
     --> Content goes here 
    </main>
    <SubMain/>

    <Footer/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import SubMain from "./components/SubMain.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
    SubMain,
  },
};
</script>

<style lang="scss">
@import './style/general.scss';
@import './style/common.scss';
@import './style/variables.scss';

main{
  // TEST
  height: 100px;
  background-color: black;
  color: white;
}

</style>
