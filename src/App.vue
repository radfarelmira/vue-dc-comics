<template>
  <div id="app">
    <Header/>

    <main>
      <section class="jumbotron">
        <img src="./assets/img/jumbotron.jpg" alt="jumbotron">
      </section>

    <SeriesList/>

    <SubMain/>
    </main>
    

    <Footer/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import SubMain from "./components/SubMain.vue";
import SeriesList from "./components/SeriesList.vue";

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

main{
  .jumbotron{
    height: 40vh;
    overflow: hidden;
  }
}


</style>
