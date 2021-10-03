<template>
  <div class="container-fluid">
      <div class="envato">
          <div class="work">
            <h2>LET'S WORK TOGETHER</h2>
            <div class="line"></div>
            <p class="p-t-35">We work as a single united team with market leading firms around the world and give our clients the highest quality advice possible.</p>
            <div class="make p-t-35">
                <span>MAKE ENQUIRY</span>
            </div>
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
    height: 400px;
    background-image: url("../assets/img/where-we-work-parallax.jpg");
    background-position: 50% 50%;
    background-repeat: no-repeat;
    color:$color-White;
    display: flex;
    flex-direction: column;
    justify-content: center;
    work{
        width: 50%;
        margin: 0 auto;
        p{
            padding: 20px;
        }
    }
}

.line {
    width: 7%;
    margin: 0 auto;
    border-bottom:1px solid $color-French-Gray;
    padding-bottom: 30px;
}

.make {
    span {
        cursor: pointer;
        padding: 10px 20px;
        background-color:$color-Breaker-Bay;
    }
}

</style>