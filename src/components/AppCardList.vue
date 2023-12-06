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
        <div class="text text-center ">
            <div class="title-section d-flex justify-content-center align-center">
                <hr style="width:20%;text-align:left;margin-left:5px;">
                <h2 class="text-center pt-5 mt-5">Featured Products</h2>
                <hr style="width:20%;text-align:right;margin-left:0">

            </div>
            <div class="buttons">
                <button type="button" class="btn btn-secondary">Men</button>
                <button type="button" class="btn btn-secondary">Women</button>
                <button type="button" class="btn btn-secondary">Accessories</button>
            </div>
        
        </div>
        <div class="row">
            <div v-for="item in images" class="col">
                <AppCard :item="item" />
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.title-section {
    align-items: center;
    vertical-align: middle;

    h2 {
        padding-bottom: 5rem;
        padding-left: 1rem;
        padding-right: 1rem;
    }

}
.buttons {
    .btn{
        background-color: hsl(0deg 0% 96.47%);
        border-radius: 0px;
        color: black;
        border: 1px solid  hsl(0, 0%, 80%);
        margin-bottom: 2rem;
        &:hover{
            background-color: white;
        }
    }
   
}

</style>

