<script>
export default {
    props: {
        item: Object
    },
    data() {
        return {

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
    <div class="card" style="width: 18rem;">
        <img :src="getImagePath(item.path)" alt="">
        <div class="card-body">
            <div class="card-text">
                <h6>{{ item.title }}</h6>
                <p>{{ item.subtitle }}</p>
                <p class="price">{{ item.price }}</p>
            </div>
        </div>
        <div class="info">
            <h5 class="text-center">Discover the quality of our products!</h5>
            <p class="fst-italic">
                The look, feel, and durability of a fabric all vary depending on its overall composition. For example, silk,
                linen, and wool all have very different and distinct properties and price ranges. A high quality silk
                garment will feel different than a high quality linen.</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    border: none;
    position: relative;


    .info {
        color: rgb(174, 174, 174);
        position: absolute;
        left: 20px;
        top: 60px;
        display: none;

        h5 {
            color: rgb(0, 0, 0);
            font-size: large;
            padding-bottom: 5rem;
        }
    }

    &:hover {
        img {
            opacity: 0;
        }

        .card-body {
            opacity: 0;
        }

        // transition: 1s;
        .info {
            display: block;
        }


    }





}


img {
    max-width: 70%;
}</style>