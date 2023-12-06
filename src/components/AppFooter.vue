<script>

export default {
    data() {
        return {
            infoList: [
                {
                    text: "12345 North Main street",
                },
                {
                    text: "New York, NY 555555",
                },
                {
                    text: "Phone:1.800.555.6789",
                },
                {
                    text: "Email: info@company.com",
                },
                {
                    text: "Web: Theme-fusion.com",
                },
            ],
            topProducts: [
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
            posts: [
                {
                    text: "Lorem ipsum dolor sit amet consectetur",
                },
                {
                    text: "Lorem ipsum dolor sit amet consectetur",
                },
                {
                    text: "Lorem ipsum dolor sit amet consectetur",
                },
                {
                    text: "Lorem ipsum dolor sit amet consectetur",
                },
                {
                    text: "Lorem ipsum dolor sit amet consectetur",
                },
                {
                    text: "Lorem ipsum dolor sit amet consectetur",
                }
            ],
            tags: ["black", "boots", "brown", "casual", "D&G", "fabric", "Flowers", "Grey", "hat", "Hipster", "lines", "multi-porpouse", "New York", "Outdoors", "red", "responsive", "summer", "sweater", "Travel", "Warm", "White", "winter",]
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
    <footer>
        <div class="footer-top">
            <div class="container d-flex">
                <div class="info-list">
                    <img src="../assets/image/images/classic_shop_logo_footer.png" alt="">
                    <ul>
                        <li v-for="item in infoList">
                            <p>{{ item.text }}</p>
                        </li>
                        <li>
                            <div class="icons d-flex gap-3">
                                <i class="fa-brands fa-facebook-f"></i>
                                <i class="fa-brands fa-twitter"></i>
                                <i class="fa-brands fa-instagram"></i>
                                <i class="fa-brands fa-youtube"></i>
                            </div>
                        </li>
                    </ul>

                </div>
                <div class="top-prod">
                    <h5>TOP RATED PRODUCTS </h5>
                    <ul>
                        <li class="d-flex" v-for="item in topProducts">
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
                <div class="posts">
                    <h5>RECENT POSTS</h5>
                    <ul>
                        <li v-for="item in posts">
                            <p>{{ item.text }}</p>
                        </li>
                    </ul>

                </div>
                <div class="tags-list">
                    <h5>TAGS</h5>
                    <div class="tag-item">
                        <span v-for="(item) in tags">{{ item }} </span>
                    </div>

                </div>
            </div>
        </div>

        <div class="footer-bottom">
            <div class="container">
                <ul d-flex flex-column justify-content-center>
                    <li>© Copyright 2012 - 2020</li>
                    <li>|</li>
                    <li>Avada Theme by Theme fusion</li>
                    <li>|</li>
                    <li>All Rights Reserved</li>
                    <li>|</li>
                    <li>Powered by WordPress </li>
                </ul>
                <img src="../assets/image/images/payment_cards_footer.png" alt="">
            </div>


        </div>

    </footer>
</template>

<style lang="scss" scoped>
.footer-top {
    background-color: hsl(214.29deg 7.53% 18.24%);
    padding: 3rem;

    h5 {
        color: hsl(0, 0%, 100%);
        text-align: center;
    }

    ul {
        margin-top: 2rem;


        li {

            list-style-type: none;
            color: hsl(0, 0%, 100%);

        }
    }
  


    .top-prod {

        li {
            display: flex;
            flex-direction: row-reverse;
            justify-content: space-between;
            border-bottom: .5px solid hsl(0deg 0% 64.71%);
            padding: 1rem;
            list-style-type: none;
            color: white;
            &:hover {
                background-color: hsl(0, 0%, 21%);
            }

            img {
                width: 80px;
                height: 90px;
            }

            .stars {
                color: cornflowerblue;

                .text {
                    color: hsl(0, 0%, 100%);
                }
            }
        }
    }

    .posts {
        li {
            border-bottom: .5px solid hsl(0deg 0% 64.71%);
            line-height: 50px;
        }

    }

    .tags-list {
        .tag-item {
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            flex-flow: wrap;
            justify-content: left;
            width: 204px;
            margin-left: 3rem;
            color: hsl(0, 0%, 100%);
        }

        span {
            border: .3px solid hsl(0deg 0% 64.71%);
            padding: .5rem;
            align-items: stretch;
            &:hover{
                background-color:hsl(0deg 0% 64.71%) ;
            }


        }

    }
}
.footer-bottom{
    background-color: hsl(216deg 7.94% 12.35%);
    height: 200px;
    padding-top: 65px;
    text-align: center;
    ul{
        display: flex;
        justify-content:space-around;
        
        li{
            list-style-type: none;
            color: white;
          
        }
    }
    
}


</style>