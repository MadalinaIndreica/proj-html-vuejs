<script>
export default {

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
                <div class="navbar-nav d-flex flex-row align-items-baseline gap-4">
                    <a class="nav-link active text-white" aria-current="page" href="#">Home<i class="fa-solid fa-chevron-down"></i></a>
                    <a class="nav-link" href="#">Shop<i class="fa-solid fa-chevron-down"></i></a>
                    <a class="nav-link" href="#">Products<i class="fa-solid fa-chevron-down"></i></a>
                    <a class="nav-link disabled" aria-disabled="true">Categories<i class="fa-solid fa-chevron-down"></i></a>
                    <a class="nav-link" href="#">News<i class="fa-solid fa-chevron-down"></i></a>
                    <a class="nav-link disabled" aria-disabled="true">Elements<i class="fa-solid fa-chevron-down"></i></a>
                    <button type="button" class="btn btn-primary">SHOP NOW!</button>
                    <i class="fa-solid fa-magnifying-glass"></i>
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
            border-right: 1px solid hsl(210deg 5.43% 36.08%);
            padding: 1rem;
        }
    }

    color: hsl(210deg 5.43% 36.08%);

    .cart {
        color: rgb(15, 15, 15);
    }

    .header-bottom {

        .logo {
            img {
                width: 200px;
            }
        }
    }
}</style>