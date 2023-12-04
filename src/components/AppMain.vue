<script>
import AppCardList from "./AppCardList.vue"
export default {
    data(){
        return{
           
        }
        
    },
    components : { AppCardList }
}

</script>

<template>
    <!-- Hero section -->
    <section class="hero py-5 mt-5">
        <h1>Brand new arrivals</h1>
        <h3>NEW COLLECTION FROM NEW YORK</h3>
        <button type="button" class="btn btn-outline-light">VIEW ALL</button>
        <button type="button" class="btn btn-outline-light">LOOK BOOK</button>
    </section>
    <!-- /Hero section -->

    <!-- Featured products -->
    <AppCardList/>
    <!-- /Featured products -->
</template>

<style lang="scss" scoped>
.hero {
    text-align: center;
    color: white;
    background-image:url(../assets/image/images/home1_slide_three_bg_2.jpg);
    background-size: cover;
    height: 400px;
    .btn{
        border-radius: 20px;
        margin-right: 20px;
    }
}

</style>