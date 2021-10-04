<template>
  <div class="container-fluid" id="app">
    <Header id="navbar"/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');
@import "./style/Utilitis.scss";
@import "./style/Colors.scss";

#navbar {
  background-color: $color-White;
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  position: sticky;
  width: 100%;
}

</style>
