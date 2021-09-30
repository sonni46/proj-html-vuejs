<template>
  <div class="container-fluid" id="app">
    <div class="container">
      <Header/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
// import Main from './components/Main.vue'
// import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    // Main,
    // Footer
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');
@import "./style/Utilitis.scss";
@import "./style/Colors.scss";

</style>
