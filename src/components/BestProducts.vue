<script>
export default {
    data() {
        return {
            cards: [
                {
                    id: 1,
                    path: 'spring_printed_dress.jpg',

                },
                {
                    id: 2,
                    path: 'modern_love_tee.jpg',

                },
                {
                    id: 3,
                    path: 'blue_jacket_and_white_stripe_tee-200x260.jpg',

                },
                {
                    id: 4,
                    path: 'blue_leather_jacket-200x260.jpg',

                },
                {
                    id: 5,
                    path: 'hipster_black_top.jpg',

                },
                {
                    id: 6,
                    path: 'black_leather_suit-200x260.jpg',

                },
             
            ],
            activeIndex:0,
        };
    },

    methods: {
        getImagePath(image) {
            return new URL(`../assets/image/images/${image}`, import.meta.url).href;
        },
    },
};

</script>

<template>
    <div class="container">
        <h2 class="text-center pt-5 mt-5">Best seller</h2>
        <p class="text-center mb-5">Must have products from our top sellers</p>
        <div class="wrapper d-flex  overflow-auto justify-content-between">
            <div class="card h-100"  v-for="card in cards" :key="card.id">
                <img :src="getImagePath(card.path)" alt="card">
            </div>
            <div class="next"><i class="fa-solid fa-chevron-right"></i></div>
            <div class="prev"><i class="fa-solid fa-chevron-left"></i></div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.wrapper{
    position: relative;
}
.prev, .next {
    
    text-align: center;
    width: 40px;
    height: 80px;
    margin: 10px 0;
    background: #333333;
    color: white;
    position: absolute;
    top: 36%;
    left: 10%;
    transform: translate(-50%);
    cursor: pointer;
    z-index: 999;
    opacity: 30%;
    padding-top: 25px;
    i {
        margin-top: 2px;
    }
}
.next {
    left: 96%;
}
.wrapper{
    padding: 6rem;
}
.card{
    border: none;
   
}
img {
    width: 250px;
}

</style>