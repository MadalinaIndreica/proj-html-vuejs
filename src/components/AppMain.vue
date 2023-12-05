<script>
import AppCardList from "./AppCardList.vue"
import BestProducts from "./BestProducts.vue";
import ListGroup from "./ListGroup.vue";

export default {
    data() {
        return {
            titleTwo: "new arrivals"
        }

    },
    components: { AppCardList, BestProducts, ListGroup }
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
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maxime accusamus quia, obcaecati facere doloribus
                praesentium.</p>
            <button type="button" class="btn btn-outline-light">VIEW MORE</button>

        </div>
        <div class="col second-col">
            <h3>Free Shipping</h3>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maxime accusamus quia, obcaecati facere doloribus
                praesentium.</p>
            <button type="button" class="btn btn-outline-light">VIEW MORE</button>
        </div>
    </div>
    <!-- /discount section -->

    <!-- new arrivals -->
    <BestProducts />
    <!-- /new arrivals-->

    <!-- profile section -->
    <div class="section  text-center">
        <div class="container">
            <img class="rounded-img" src="../assets/image/images/woman_testimonial.png" alt="">
            <p class="fst-italic">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio error debitis, modi
                recusandae possimus vel aperiam fuga illo unde alias, quasi vero ullam aut ex omnis dolore voluptatem
                libero. Nemo.</p>
            <span><strong>Darío Pineda</strong> - Theme fusion.</span>
        </div>

    </div>
    <!-- /profile section -->

    <!-- From our blog -->
    <div class="container">
        <div class="blog-section">
            <div class="text-part">
                <h2 class="text-center">From Our Blog</h2>
                <p class="text-center">The latest Classic Shop news</p>
            </div>
            <!-- first card -->
            <div class="row d-flex gap-5 justify-content-center">
                <div class="card" style="width: 25rem;">
                    <img src="../assets/image/images/post_img_12-200x125.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5>Lorem ipsum dolor sit, amet consectetur</h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque nisi animi eum
                            itaque deleniti ab, incidunt, nesciunt quisquam voluptates.</p>
                    </div>
                </div>

                <!-- second card -->
                <div class="card" style="width: 25rem;">
                    <img src="../assets/image/images/post_img_11-200x125.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5>Lorem ipsum dolor sit, amet consectetur</h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque nisi animi eum
                            itaque deleniti ab, incidunt, nesciunt quisquam voluptates.</p>
                    </div>
                </div>

                <!-- third card -->
                <div class="card" style="width: 25rem;">
                    <img src="../assets/image/images/post_img_10-200x125.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5>Lorem ipsum dolor sit, amet consectetur</h5>
                        <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque nisi animi eum
                            itaque deleniti ab, incidunt, nesciunt quisquam voluptates.</p>
                    </div>
                </div>
            </div>
        </div>

    </div>
    <!-- /From our blog -->

    <hr>

    <!-- list group -->
    <ListGroup />
    <!-- /list group -->

    <!-- logo section -->
    <div class="logo-section">
        <div class="container">
            <h2 class="text-center">BRAND LOGOS</h2>
            <div class="logos d-flex justify-content-between">
                <div class="logo-image">
                    <img src="../assets/image/images/b_logotype_1.png" alt="">
                </div>
                <div class="logo-image">
                    <img src="../assets/image/images/b_logotype_2.png" alt="">
                </div>
                <div class="logo-image">
                    <img src="../assets/image/images/b_logotype_3.png" alt="">
                </div>
                <div class="logo-image">
                    <img src="../assets/image/images/b_logotype_4.png" alt="">
                </div>
                <div class="logo-image">
                    <img src="../assets/image/images/b_logotype_5.png" alt="">
                </div>
            </div>
        </div>
    </div>
    <!-- /logo section -->

    <!-- input section -->
    <div class="input-section">
        <div class="container d-flex  justify-content-evenly">
            <div class="subscribe d-flex justify-content-evenly">
                <i class="fa-regular fa-envelope "></i>
                <h2>Subscribe now and get special offers</h2>
            </div>
            <div class="input-part d-flex justify-content-between">
                <label for="exampleFormControlInput1" class="form-label"></label>
                <input type="email" class="form-control form-control-lg" id="exampleFormControlInput1" placeholder="insert your email">
                <button type="submit" class="btn btn-primary mb-3">SEND</button>
            </div>
        </div>
    </div>
    
    <!-- /input section -->
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
        background-color: hsl(214.83deg 60.85% 53.92%);
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

    .col {
        text-align: center;
        background-size: cover;
        height: 350px;

        h3 {
            margin-top: 100px;
        }
    }

    .first-col {
        background-image: url(../assets/image/images/promo_box_1_bg.jpg);
    }

    .second-col {
        background-image: url(../assets/image/images/promo_box_2_bg.jpg);
    }
}

// profile section
.section {
    color: white;
    background-image: url(../assets/image/images/testimonials_home_1_bg.jpg);
    background-size: cover;
    height: 400px;

    .rounded-img {
        margin-top: 100px;
        margin-bottom: 15px;
        width: 100px;
        height: 100px;
        object-fit: cover;
        border-radius: 50%;
    }
}

//  From our blog
.blog-section {

    .text-part {
        margin-top: 100px;
        margin-bottom: 50px;

    }

    .card {
        border: none;
    }
}

hr {
    margin-top: 5rem;
}

// logo section
.logo-section {

    background-color: hsl(0deg 0% 96.47%);
    height: 400px;
    padding: 5rem;

    h2 {
        color: hsl(0deg 0% 64.71%);
        padding-bottom: 4rem;
    }
}

// input section
.input-section {
    background-color: hsl(214.29deg 6.8% 20.2%);
    color: white;
    height: 300px;
   vertical-align: middle;
   padding-top: 7rem;
    .fa-envelope {
        width: 50px;
        height: 50px;
        background-color:hsl(214.29deg 7.53% 18.24%);;
        border-radius: 50%;
        text-align: center;
        padding-top: 15px;
    }
    .form-control-lg {
        border-radius: 35px;
    }
    .btn {
        background-color: hsl(214.83deg 60.85% 53.92%);
        border-radius: 20px;
        margin-top: 1rem;
    }
}
</style>