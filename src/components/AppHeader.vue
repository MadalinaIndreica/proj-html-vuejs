<script>
export default {
    props: {
        navItems: Array,
    }
}
</script>

<template>
    <header>
        <div class="container">
            <!-- HEADER TOP -->
            <div class="header-top d-flex justify-content-between align-items-center">
                <div class="icons d-flex gap-3">
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-instagram"></i>
                    <i class="fa-brands fa-youtube"></i>
                </div>
                <div class="user-account d-flex gap-3">
                    <span>Shopping Cart</span>
                    <span>My Account</span>
                    <span class="cart"><i class="fa-solid fa-cart-shopping"></i>Cart</span>
                </div>

            </div>
            <!-- /HEADER TOP -->
            <!-- HEADER BOTTOM -->
            <div class="header-bottom d-flex justify-content-between align-items-center mt-3">
                <div class="logo">
                    <img src="../assets/image/images/classic_shop_logo2x.png" alt="">
                </div>
                <div class="navbar-nav">
                    <ul class="navbar-nav d-flex flex-row align-items-baseline gap-4">
                        <li v-for="item in navItems"><a href="">{{ item }}<i class="fa-solid fa-chevron-down"></i></a></li>
                        <button type="button" class="btn btn-primary">SHOP NOW!</button>
                        <i class="fa-solid fa-magnifying-glass"></i>
                    </ul>
                </div>
            </div>
            <!--/ HEADER BOTTOM -->
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    .header-top {
        height: 60px;
        border-bottom: 1px solid hsl(210deg 5.43% 36.08%);

        span {
          
            padding: 1rem;
            &:hover{
                background-color: rgb(50, 135, 255);
                opacity:1;
                color: white;

            }
        }
    }



    .cart {
        color: rgb(15, 15, 15);
    }

    .header-bottom {
        i{
            margin-left: 5px;
        }
        a {
            text-decoration: none;
            color: hsl(210deg 5.43% 36.08%);
            

            &:hover {
               border-top:5px solid rgb(50, 135, 255);
               padding: 2rem;
               transition: .5s
            }

        }

        .logo {
            img {
                width: 200px;
            }
        }
    }
}
</style>