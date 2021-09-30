<template>
  <div class="jumbo container-fluid bg-Ebb">
      <img :src="require(`@/assets/img/video_law_home_preview.jpg`)" alt="">
  </div>
</template>

<script>

export default {
    name:"Jumbo",
}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";
.jumbo{
    img {
        width: 100%;
        height: 600px;
        object-fit: cover;
        object-position: top;
    }
}
</style>