<script>
export default {

}
</script>

<template>
    <header>
        <div class="container">
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
            <div class="header-bottom">

            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header{
    .header-top {
        height: 60px;
        border-bottom: 1px solid hsl(210deg 5.43% 36.08%) ;
        span{
            border-right: 1px solid hsl(210deg 5.43% 36.08%);
            padding: 1rem;
        }
    }
   color: hsl(210deg 5.43% 36.08%);
   .cart {
    color: rgb(15, 15, 15);
   }
}
</style>