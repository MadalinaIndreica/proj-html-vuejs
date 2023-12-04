<script>
import AppCard from './AppCard.vue';


export default {
    components: {
        AppCard,

    },
    data() {
        return {
            images: [
                {
                    path: 'black_elegant_leather_jacket-231x300.jpg',
                    title: 'Black Leather Jacket',
                    subtitle: 'Men, jackets',
                    price: '$200'
                },
                {
                    path: 'black_leather_suit-200x260.jpg',
                    title: 'Black Leather suit',
                    subtitle: 'Men, jackets, suits',
                    price: '$176'
                },
                {
                    path: 'blue_jacket_and_white_stripe_tee-200x260.jpg',
                    title: 'Black Jackett & Stripe tee',
                    subtitle: 'Men, jackets',
                    price: '$580'
                },
                {
                    path: 'blue_leather_jacket-200x260.jpg',
                    title: 'Modern Black Jacket Suit',
                    subtitle: 'Men, jackets',
                    price: '$96'

                }
            ]
        }
    }
}

</script>

<template>
    <div class="container">
        <div class="text text-center m-5">
        <h2>Featured Products</h2>
        <h6>must have products from our top sellers</h6>
        </div>
        <div class="row">
            <div v-for="item in images" class="col">
                <AppCard :item="item" />
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>


</style>

