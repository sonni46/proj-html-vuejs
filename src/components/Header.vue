<template>
  <div class="d-flex justify-content-between">
    <div>
      <img :src="require(`@/assets/img/avada-law-logo.png`)" alt="">
    </div>
    <div class="">
      <ul class="d-flex align-items-center">
        <li v-for="(info,index) in infoMenu" :key="index">
          <a href="">{{info.message}}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name : "Header",
  data(){
   return {
      infoMenu: [
                {message:'Home'},
                {message:'Who We Are'},
                {message:'Who We Do'},
                {message:'Where We Work'},
                {message:'Careers'},
                {message:'News'},
                {message:'Contact'}],
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/Colors.scss";
@import "@/style/Utilitis.scss";

ul {
  width: 100%;
  height: 100%;
  list-style: none;
    li {
      padding: 0 10px;
        a {
          color: $color-Shark;
          text-decoration: none;
        }
    }
}

</style>
