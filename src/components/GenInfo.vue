<template>
  <div class="bg-Ebb container-fluid pad-50">
        <div class="container">
            <div>
                <ul class="d-flex bg-white border-t-Nymph">
                    <li class="p-y-15 p-x-50">
                        <h3 class="p-y-15 p-t-35">WHO WE ARE</h3>
                        <span>Ipsa sint ex dolorum autem non reprehenderit neque, harum vitae!
                            Ipsa sint ex dolorum autem non reprehenderit neque, harum vitae!
                        </span>
                        <div class=" p-y-35 p-b-50">
                            <span class="button">LEARN MORE</span>
                        </div>
                    </li>
                    <li class="p-y-15 p-x-50">
                        <h3 class="p-y-15 p-t-35">WHAT WE DO </h3>
                        <span>Ipsa sint ex dolorum autem non reprehenderit neque, harum vitae!
                            Ipsa sint ex dolorum autem non reprehenderit neque, harum vitae!
                        </span>
                        <div class=" p-y-35 p-b-50">
                            <span class="button">LEARN MORE</span>
                        </div>
                    </li>
                    <li class="p-y-15 p-x-50">
                        <h3 class="p-y-15 p-t-35">WHERE WE WORK</h3>
                        <span>Ipsa sint ex dolorum autem non reprehenderit neque, harum vitae!
                            Ipsa sint ex dolorum autem non reprehenderit neque, harum vitae!
                        </span>
                        <div class=" p-y-35 p-b-50">
                            <span class="button">LEARN MORE</span>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "GenInfo",
}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import "@/style/Utilitis.scss";
@import "@/style/Colors.scss";

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

.button {
    cursor: pointer;
    padding:10px 20px;
    background-color:$color-Shark ;
    color:$color-White;
}


</style>