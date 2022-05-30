<template>
    <div class="v-gallery-item">
        <img :src="require(`../assets/gallery/${props.image}`)" alt="image" class="gallery-item">
<!--        <img :src="require(`../assets/gallery/mobile/${props.image}`)" alt="image" class="gallery-mobile-item">-->
    </div>
</template>

<script setup>
import {defineProps} from 'vue'

const props = defineProps({
    image: {
        type: String
    }
})
</script>

<style lang="scss" scoped>
.v-gallery-item {
    background: #ffff;
    border: 1px solid black;
    border-radius: 30px;
    padding: 1rem;
    margin: 1rem;
    display: inline-block;
    .gallery-item {
        border-radius: 30px;
        max-width: 100%;
        height: auto;
    }
    //.gallery-mobile-item {
    //    display: none;
    //}
}

@media only screen and (max-width: 428px) {
    .v-gallery-item {
        padding: 1rem;
        margin: 2rem 0 0 0;
        display: inline-block;
        //.gallery-item {
        //    display: none;
        //}
        //.gallery-mobile-item {
        //    display: block;
        //}
    }
}
</style>