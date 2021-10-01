<template>
  <div class="challenge pad-y-100">
      <div class="p-b-50">
          <h2>GLOBAL CHALLENGE. WORLD CLASS RESPONSE</h2>
          <div class="line"></div>
      </div> 
      <div class="container">
        <div class="camp d-flex justify-content-between">
            <!-- PEOPLE -->
            <div class="p-r-20">
                <h4>OUR PEOPLE</h4>
                <div>
                    <ul class="box">
                        <li v-for="people,index in peoples" :key="index">
                            <div class="d-flex align-items-center bg-Ebb">
                                <img class="p-15" :src="require(`../assets/img/${people.img}`)" alt="">
                                <strong><span>{{people.name}}</span></strong>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- PEOPLE -->

            <!-- PRACTICE AREAS -->
             <div class="p-r-20">
                <h4>OUR PRACTICE AREAS</h4>
                <div>
                    <ul class="box">
                        <li class="" v-for="(prat,index) in practices" :key="index">
                            <div class="d-flex align-items-center bg-Ebb">
                                <img class="p-15" :src="require(`../assets/img/${prat.img}`)" alt="">
                                <strong><span>{{prat.name}}</span></strong>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- PRACTICE AREAS -->

            <!-- PUBLICATIONS -->
             <div class="p-r-20">
                <h4>OUR PUBLICATIONS</h4>
                <div>
                    <ul class="box">
                        <li class="" v-for="(pub,index) in pubblications" :key="index">
                            <div class="d-flex align-items-center bg-Ebb">
                                <img class="p-15" :src="require(`../assets/img/${pub.img}`)" alt="">
                                <strong><span>{{pub.name}}</span></strong>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- PUBLICATIONS -->
          </div>
      </div>
  </div>
</template>

<script>
import * as people from "@/js/Info.js";
import * as practice from "@/js/Info.js";
import * as pubblication from "@/js/Info.js";
export default {
    name: "Challenge",
    data() {
        return{
            peoples:people.people,
            practices:practice.practice,
            pubblications:pubblication.pubblication
        }
    }

}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";

.challenge {
    .camp {
        width: 100%;
        h4 {
            margin-bottom: 15px;
        }
    }

    ul{
        list-style: none;
        li{
            margin-bottom: 15px;
            div {
                font-size: 12px;
                padding-right:150px;
                
            }
        }
    }
    h2{
        padding-bottom: 30px;
        text-align: center;
    }
    img{
        width: 80px;
    }
}

.line {
    width: 7%;
    margin: 0 auto;
    border-bottom:1px solid $color-French-Gray;
}
</style>