<template>
  <div class="container-fluid">
      <div class="envato">
          <div>
            <img :src="require(`@/assets/img/envato-logo.png`)" alt="">
            <p>"We have worked with Avada Law for the past 15 years. As we have grown and evolved, what I have valued most about our relationship is that Avada Law know us and our business."</p>
            <p>Nigel Rawlinson • Senior Partner</p>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";
.envato {
    text-align: center;
    width: 100%;
    height: 300px;
    background-image: url("../assets/img/showeare-parallax.jpg");
    background-position: 50% 60%;
    background-size: 120%;
    background-repeat: no-repeat;
    color:$color-White;
    div{
        width: 50%;
        margin: 0 auto;
        padding-top: 100px;
        p{
            padding: 20px;
        }
    }

}

</style>