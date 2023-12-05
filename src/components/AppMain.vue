<script>
import AppCardList from "./AppCardList.vue"
import BestProducts from "./BestProducts.vue";

export default {
    data() {
        return {

        }

    },
    components: { AppCardList, BestProducts, }
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
        <div class="row my-5">
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

    <!-- best products section -->
    <BestProducts />
    <!-- best products section -->

    <!-- discount section -->
    <div class="row discount">
        <div class="col first-col">
            <h3>70% Off</h3>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maxime accusamus quia, obcaecati facere doloribus praesentium.</p>
            <button type="button" class="btn btn-outline-light">VIEW MORE</button>

        </div>
        <div class="col second-col">
            <h3>Free Shipping</h3>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maxime accusamus quia, obcaecati facere doloribus praesentium.</p>
            <button type="button" class="btn btn-outline-light">VIEW MORE</button>
        </div>
    </div>
    <!-- /discount section -->
</template>

<style lang="scss" scoped>
.hero {
    text-align: center;
    color: white;
    background-image: url(../assets/image/images/home1_slide_three_bg_2.jpg);
    background-size: cover;
    height: 400px;

    .hero-text {
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

// discount section
.discount {
    background-image: url(../assets/image/images/bkgd_confetti-compressor.jpg);
    background-size: cover;
    height: 500px;
    padding: 4rem;
    gap: 2rem;
    .col{
        text-align: center;
        background-size: cover;
        height: 350px;
        h3{
            margin-top: 100px;
        }
    }
    .first-col{
        background-image:url(../assets/image/images/promo_box_1_bg.jpg) ;
    }
    .second-col {
        background-image: url(../assets/image/images/promo_box_2_bg.jpg);
    }
}
</style>