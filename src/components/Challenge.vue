<template>
  <div class="challenge pad-y-100">
      <div>
          <h3>GLOBAL CHALLENGE. WORLD CLASS RESPONSE</h3>
      </div> 
      <div>
          <div class="container">
              <h4>OUR PEOPLE</h4>
              <div>
                  <ul class="box">
                      <li>
                        <img :src="require(`../assets/img/column1-image1.jpg`)" alt="">
                        <span>Deborah Brown</span>
                      </li>
                  </ul>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "Challenge",

}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";

.challenge {
    ul{
        list-style: none;
    }
    h3 {
        text-align: center;
    }
}
</style>