<template>
<div>
  <div class="bg-Ebb container-fluid pad-y-100">
        <div class="container">
            <div class="learn">
                <ul class="d-flex bg-white border-t-Nymph">
                    <li class="p-y-15 p-x-50">
                        <h3 class="p-y-15 p-t-35">WHO WE ARE</h3>
                        <span>Nullam fringilla tristique elit id varius.Nulla lacina quanm nec venenatis dignissim.Vivamus volutpat tempus semper. Cras feugiat mi sit amet risus consectetur.
                        </span>
                        <div class=" p-y-35 p-b-50">
                            <span class="button">LEARN MORE</span>
                        </div>
                    </li>
                    <li class="p-y-15 p-x-50 center">
                        <h3 class="p-y-15 p-t-35">WHAT WE DO </h3>
                        <span>Nullam fringilla tristique elit id varius.Nulla lacina quanm nec venenatis dignissim.Vivamus volutpat tempus semper. Cras feugiat mi sit amet risus consectetur.
                        </span>
                        <div class=" p-y-35 p-b-50">
                            <span class="button">LEARN MORE</span>
                        </div>
                    </li>
                    <li class="p-y-15 p-x-50">
                        <h3 class="p-y-15 p-t-35">WHERE WE WORK</h3>
                        <span>Nullam fringilla tristique elit id varius.Nulla lacina quanm nec venenatis dignissim.Vivamus volutpat tempus semper. Cras feugiat mi sit amet risus consectetur.
                        </span>
                        <div class=" p-y-35 p-b-50">
                            <span class="button">LEARN MORE</span>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
    <div  class="container">
        <ul class="d-flex global pad-y-100">
            <li v-for="(global,index) in globals" :key="index">
                <i class="fas fa-check"></i>
                <h3 class="p-y-15">{{global.message}}</h3>
                <span>Nullam fringilla tristique elit id varius.Nulla lacina quanm nec venenatis dignissim.
                </span>
            </li>
        </ul>  
    </div>
    <div class="ask">
        <div class="container p-y-50 d-flex align-items-center justify-content-between"> 
            <h3>QUESTIONS ABOUT A JUDICAL ISSUE? ASK OUR EXPERTS</h3>
            <span>ASK AN EXPERT</span>
        </div>
    </div>
</div>
</template>

<script>
import * as global from "@/js/Info.js";
export default {
    name: "GenInfo",
    data(){
        return{
            globals:global.global
        }
    }
}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";

.container-fluid {
    border-bottom:1px solid $color-French-Gray;
}

.learn {

    ul {
        list-style: none;
        text-align: center;
        border-left:1px solid $color-French-Gray;
        border-bottom:1px solid $color-French-Gray;
        border-right:1px solid $color-French-Gray;
        .center {
            border-left:1px solid $color-French-Gray;
            border-right:1px solid $color-French-Gray;
        }
    }
}

.button {
    cursor: pointer;
    padding:10px 20px;
    background-color:$color-Shark ;
    color:$color-White;
}

.global {
    list-style: none;
    text-align: center;
    i {
        color:$color-Breaker-Bay ;
    }
}

.ask {
    background-color:$color-Breaker-Bay;
    color:$color-White;
    span {
        padding: 10px 20px;
        background-color:$color-Sea-Nymph;
    }
}


</style>