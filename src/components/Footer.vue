<template>
<div class="container  p-y-35 ">
    <div>
        <h2>CALL OUR EXPERTS TODAY 1.800.555.6789</h2>
    </div>
   <div class="d-flex justify-content-between footer align-items-center">
       <div class="footer-mes">
           <span v-for="(foot,index) in Footer" :key="index">
                {{foot.message}}
           </span>
       </div>
       <div class="social">
            <a href="">
                <i class='bg-Bay pad-fb color-White fab fa-facebook-f'></i>
            </a>
            <a href="" v-for="(social,index) in SocialsList" :key="index" >
                <i class='bg-Bay pad-10 color-White' :class="social.icon"></i>
            </a>
        </div>
    </div>
</div>
</template>

<script>
import * as socials from "@/js/Info.js";
import * as footer from "@/js/Info.js";
export default {
    name: "Footer",
     data(){
        return {
            SocialsList:socials.socials,
            Footer:footer.footer
        }
    },
}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";

.social {
    i {
        border-radius: 18%;
        margin-right: 10px;
    }
}
.pad-10 {
        padding: 10px 10px;
    }

.pad-fb {
    padding: 10px 13px;
}

.footer {
    width: 100%;
    margin-top: 20px;
}

.footer-mes {
    font-size: 12px;
}

</style>