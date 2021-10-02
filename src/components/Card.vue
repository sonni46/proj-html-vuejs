<template>
  <div class="container-fluid bg-Ebb pad-y-100">
      <div class="container">
            <div class="learn">
                <ul class="d-flex bg-white border-t-Nymph">
                    <!-- Card 1 -->
                    <li class="p-y-15 p-x-50">
                        <div class="p-b-50">
                            <img class="p-t-35" :src="require(`@/assets/img/law_7.jpg`)" alt="">
                            <h3 class="p-y-15 p-t-35">WHO WE ARE</h3>
                            <span>Nullam fringilla tristique elit id varius.Nulla lacina quanm nec venenatis dignissim.Vivamus volutpat tempus semper. Cras feugiat mi sit amet risus consectetur.
                            </span>
                        </div>
                    </li>
                    <!-- Card 1 -->

                    <!-- Card 2 -->
                    <li class="p-y-15 p-x-50 center">
                        <div class="p-b-50">
                            <img class="p-t-35" :src="require(`@/assets/img/law_8.jpg`)" alt="">
                            <h3 class="p-y-15 p-t-35">WHAT WE DO </h3>
                            <span>Nullam fringilla tristique elit id varius.Nulla lacina quanm nec venenatis dignissim.Vivamus volutpat tempus semper. Cras feugiat mi sit amet risus consectetur.
                            </span>
                        </div>
                    </li>
                    <!-- Card 2 -->

                    <!-- Card 3 -->
                    <li class="p-y-15 p-x-50">
                        <div class="p-b-50">
                            <img class="p-t-35" :src="require(`@/assets/img/law_3.jpg`)" alt="">
                            <h3 class="p-y-15 p-t-35">WHERE WE WORK</h3>
                            <span>Nullam fringilla tristique elit id varius.Nulla lacina quanm nec venenatis dignissim.Vivamus volutpat tempus semper. Cras feugiat mi sit amet risus consectetur.
                            </span>
                        </div>
                    </li>
                    <!-- Card 3 -->
                </ul>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name:"Card",

}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";

ul {
    list-style: none;
    border-left:1px solid $color-French-Gray;
    border-bottom:1px solid $color-French-Gray;
    border-right:1px solid $color-French-Gray;
    li {
            img {
            width:100%;
        }
    }
}

.center {
        border-left:1px solid $color-French-Gray;
        border-right:1px solid $color-French-Gray;
}

</style>