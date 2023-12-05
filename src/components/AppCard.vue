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
    </div>
</template>

<style lang="scss" scoped>
.card{
border: none;
}
img{
    max-width: 70%;
}
</style>