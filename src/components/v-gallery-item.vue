<template>
    <div class="v-gallery-item">
        <img :src="require(`../assets/gallery/${props.image}`)" alt="image">
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
    display: inline-block;
    img {
        border-radius: 30px;
    }
}
</style>