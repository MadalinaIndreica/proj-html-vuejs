<script>
export default {
    data() {
        return {
            firstList: [
                {
                    path: "spring_printed_dress.jpg",
                    text: " Black Jacket Leather",
                    price: "$300"
                },
                {
                    path: "black_leather_suit-200x260.jpg",
                    text: " Black Jacket Leather"
                },
                {
                    path: "modern_love_tee.jpg",
                    text: " Black Jacket Leather",
                    price: "$678"
                }
            ],
            secondList: [
                {
                    path: "blue_leather_jacket-200x260.jpg",
                    text: " Black Jacket Leather",
                    price: "$500"
                },
                {
                    path: "modern_love_tee.jpg",
                    text: " Black Jacket Leather"
                },
                {
                    path: "hipster_black_top.jpg",
                    text: " Black Jacket Leather",
                    price: "$390"
                }
            ],
            thirdList: [
                {
                    path: "black_leather_suit-200x260.jpg",
                    text: " Black Jacket Leather"
                },
                {
                    path: "spring_printed_dress.jpg",
                    text: " Black Jacket Leather",
                    price: "$190"
                },
                {
                    path: "blue_leather_jacket-200x260.jpg",
                    text: " Black Jacket Leather"
                }
            ],
            fourthList: [
                {
                    path: "black_leather_suit-200x260.jpg",
                    text: " Black Jacket Leather",
                    price: "$1790"
                },
                {
                    path: "modern_love_tee.jpg",
                    text: " Black Jacket Leather"
                },
                {
                    path: "hipster_black_top.jpg",
                    text: " Black Jacket Leather",
                    price: "$190"
                }
            ]
        }
    },
   methods: {
        getImagePath(image) {
            return new URL(`../assets/image/images/${image}`, import.meta.url).href;
         }
    }
}

</script>

<template>
    
    <div class="container">
        <div class="list-section d-flex ">
            <div class="first-list">
                <h4>FREATURED</h4>
                <ul>
                    <li v-for="item in firstList">
                        <img :src="getImagePath(item.path)" />
                        <p>{{ item.text }} {{ item.price }}</p>

                    </li>
                </ul>
            </div>
            <div class="second-list">
                <h4>ON SALE</h4>
                <ul>
                    <li v-for="item in secondList">
                        <img :src="getImagePath(item.path)" />
                        <div class="stars">
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <div class="text">
                            <p>{{ item.text }} {{ item.price }}</p>
                            </div>
                        </div>

                    </li>
                </ul>
            </div>
            <div class="third-list">
                <h4>LATEST REVIEWS</h4>
                <ul>
                    <li v-for="item in thirdList">
                        <img :src="getImagePath(item.path)" />
                        <p>{{ item.text }} {{ item.price }}</p>

                    </li>
                </ul>
            </div>
            <div class="fourth-list">
                <h4>LATEST REVIEWS</h4>
                <ul>
                    <li v-for="item in fourthList">
                        <img :src="getImagePath(item.path)" />
                        <div class="stars">
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <div class="text">
                            <p>{{ item.text }} {{ item.price }}</p>
                            </div>
                        </div>

                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.list-section {
    width: 500px;
    text-align: center;
    margin-left: 30px;
    margin-top: 10rem;
    margin-bottom: 5rem;
    ul{
        padding: 2rem;
    }
    li {
        display: flex;
        flex-direction: row-reverse;
        justify-content: center;
        border-bottom: 1px solid rgb(182, 182, 182);
        padding: 1rem;

        img {
            width: 150px;
            height: 100px;
        }
        .stars {
            color: cornflowerblue;
            .text{
                color: black;
            }
        }
    }
}
</style>