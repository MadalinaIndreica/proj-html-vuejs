<script>
import AppCardList from "./AppCardList.vue"
export default {
    data() {
        return {

        }

    },
    components: { AppCardList }
}

</script>

<template>
    <!-- Hero section -->
    <section class="hero py-5 mt-5">
        <div class="hero-text">
            <h1>Brand new arrivals</h1>
            <h3>NEW COLLECTION FROM NEW YORK</h3>
            <button type="button" class="btn btn-outline-light">VIEW ALL</button>
            <button type="button" class="btn btn-outline-light">LOOK BOOK</button>
        </div>
    </section>
    <!-- /Hero section -->

    <!-- Featured products -->
    <AppCardList />
    <!-- /Featured products -->

    <!-- Collections section -->
    <div class="text-center">
        <div class="row">
            <div class="col winter-col">
                <div class="text">
                    <h4>Winter Collection</h4>
                    <p>STYLISH AND WARM</p>
                    <button type="button" class="btn btn-outline-light">VIEW MORE</button>
                </div>
            </div>
            <div class="col spring-col">
                <div class="text">
                    <h4>Spring Collection</h4>
                    <p>BRIGHT AND COLORFUL</p>
                    <button type="button" class="btn btn-outline-light">VIEW MORE</button>
                </div>
            </div>
            <div class="col autumn-col">
                <div class="text">
                    <h4>Autumn Collection</h4>
                    <p>RICH AND COMFORTABLE</p>
                    <button type="button" class="btn btn-outline-light">VIEW MORE</button>
                </div>
            </div>
        </div>
    </div>
    <!-- /Collections section -->

    <!-- carousel section -->

    <!-- carousel section -->

</template>

<style lang="scss" scoped>
.hero {
    text-align: center;
    color: white;
    background-image: url(../assets/image/images/home1_slide_three_bg_2.jpg);
    background-size: cover;
    height: 400px;
    .hero-text{
        padding-top: 100px;
    }
    .btn {
        border-radius: 20px;
        margin-right: 20px;
    }
}

// collections cols
.row {
    height: 400px;
    color: white;



    .winter-col {
        background-image: url(../assets/image/images/winter_collection_bg.jpg);
        background-size: cover;

    }

    .spring-col {
        background-image: url(../assets/image/images/spring_collection_bg.jpg);
        background-size: cover;
    }

    .autumn-col {
        background-image: url(../assets/image/images/autumn_collection_bg.jpg);
        background-size: cover;
    }

    .text {
        padding-top: 150px;
    }

}
</style>