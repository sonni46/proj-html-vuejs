<template>
<div>
    <div class="border-t-Nymph bg-Ebb">
        <div class="container d-flex align-items-center justify-content-between">
            <!-- info  -->
            <div class="p-y-15 color-Gray ">
                <span>Avada &amp; Associates legal team announce deal to open up oil &amp; gas</span>
            </div>
            <!-- info  -->

            <!-- social  -->
            <div class="social d-flex justify-content-between">
                <a href="">
                    <i class='bg-Bay pad-fb color-White fab fa-facebook-f'></i>
                </a>
                <a href="" v-for="(social,index) in SocialsList" :key="index" >
                    <i class='bg-Bay pad-10 color-White' :class="social.icon"></i>
                </a>
            </div>
            <!-- social  -->
        </div>  
    </div>
    <!-- jumbo  -->
    <Jumbo/>
    <!-- jumbo  -->

    <!-- general info  -->
    <GenInfo/>
    <!-- general info  -->
    
    <!-- Challenge -->
    <Challenge/>
    <!-- Challenge -->

    <!-- Envato -->
    <Envato/>
    <!-- Envato -->

    <!--Card -->
    <Card/>
    <!--Card -->

</div>
</template>

<script>
import GenInfo from './GenInfo.vue';
import * as socials from "@/js/Info.js";
import Jumbo from './Jumbo.vue';
import Challenge from './Challenge.vue';
import Envato from './Envato.vue';
import Card from './Card.vue';


export default {
  components: { 
      Jumbo, 
      GenInfo,
      Challenge,
      Envato,
      Card
    },
    name:"Main",
    data(){
        return {
            SocialsList:socials.socials
        }
    },
}
</script>


<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";

.social {
    width: 18%;
    i {
        border-radius: 18%;
    }
}
.pad-10 {
        padding: 10px 10px;
    }

.pad-fb {
    padding: 10px 13px;
}

</style>