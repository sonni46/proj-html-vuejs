<template>
<!-- menu  -->
<div class="">
  <div class="d-flex justify-content-between menu container">
    <div class="d-flex">
      <img :src="require(`@/assets/img/avada-law-logo.png`)" alt="">
    </div>
    <div class="">
      <ul class="d-flex align-items-center">
        <li v-for="(info,index) in infoMenu" :key="index">
          <a href="" :class="(info.active === true) ? 'active': null">{{info.message}}</a>
        </li>
      </ul>
    </div>
  </div>
</div>
<!--fine  menu  -->
</template>

<script>
import * as menu from "@/js/Info.js";
export default {
  name : "Header",
  data(){
   return {
      infoMenu: menu.menu
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/Colors.scss";
@import "@/style/Utilitis.scss";

.menu{
  padding:20px 0;
}

ul {
  width: 100%;
  height: 100%;
  list-style: none;
    li {
      padding: 0 10px;
        a {
          color: $color-Shark;
          text-decoration: none;
          padding-top: 20px;
        }
    }
}

.active {
  border-top:1px solid $color-Breaker-Bay;
  color:$color-Sea-Nymph;
}

</style>
