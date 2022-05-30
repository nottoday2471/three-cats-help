<template>
    <div class="v-gallery" id="gallery">
        <div class="v-gallery_title">
            <img src="../assets/links/Gallery-title.png" alt="gallery-title">
            <img src="../assets/links/Gallery-mobile.png" alt="gallery-title" class="gallery-mobile-title">
        </div>
        <div class="v-gallery_wrapper">
            <div class="v-gallery_wrapper_content">
                <div class="v-gallery_wrapper_content_list">
                    <v-gallery-item
                        v-for="(image, index) in images1"
                        :key="index"
                        :image="image"
                    />
                </div>
                <div class="v-gallery_wrapper_content_button">
                    <div class="v-gallery_wrapper_content_button_link">
                        <a href="https://opensea.io/collection/three-cats-help" target="_blank">
                            <div>
                                <span>See more</span>
                            </div>
                        </a>
                    </div>
                </div>
<!--                <div class="v-gallery_wrapper_content_list">-->
<!--                    <div class="list-2">-->
<!--                        <v-gallery-item-->
<!--                            v-for="(image, index) in images2"-->
<!--                            :key="index"-->
<!--                            :image="image"-->
<!--                        />-->
<!--                    </div>-->
<!--                </div>-->
            </div>
        </div>
    </div>
</template>

<script setup>
import VGalleryItem from '@/components/v-gallery-item'
import {ref} from 'vue'

let isMobile = ref(null)

const checkWidth = () => window.innerWidth <= 428

isMobile.value = checkWidth()

console.log(isMobile.value, window.innerWidth)


const images1 = isMobile.value ? [
    'mobile/1.png',
    'mobile/2.png',
    'mobile/3.png',
    'mobile/4.png',
    'mobile/5.png',
    'mobile/6.png']
    :
    [
        '1.png',
        '2.png',
        '3.png',
        '4.png',
        '5.png',
        '6.png',
        '7.png',
        '8.png']
// const images2 = isMobile.value ? [] : ['5.png', '6.png', '7.png', '8.png']
</script>

<style lang="scss" scoped>
.v-gallery {
    background: url('../assets/backgrounds/Cat-Paw-Background-Gallery.png'), #E3EBFF;
    width: 100%;
    min-height: 940px;
    padding: 1rem 0 0 0;
    &_title {
        display: flex;
        justify-content: center;
        .gallery-mobile-title {
            display: none;
        }
    }
    &_wrapper {
        display: flex;
        justify-content: center;
        padding: 2rem 0 0 0;
        margin: 2rem 0 0 0;
        &_content {
            display: flex;
            justify-content: space-between;
            flex-direction: column;
            width: 1300px;
            &_list {
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
            }
            &_button {
                display: flex;
                justify-content: center;
                margin: 2rem 0 2rem 0;
                &_link {
                    a {
                        text-decoration: none;
                        border-radius: 20px;
                        div {
                            background: #ffff;
                            border: 1px solid black;
                            border-radius: 20px;
                            padding: 1rem;
                            span {
                                font-size: 2rem;
                                color: black;
                            }
                        }
                        &:hover {
                            opacity: .6;
                        }
                    }
                }
            }
        }
    }
}

@media only screen and (max-width: 428px) {
    .v-gallery {
        height: 812px;
        &_title {
            img {
                display: none;
            }
            .gallery-mobile-title {
                display: block;
            }
        }
        &_wrapper {
            &_content {
                max-width: 350px;
                &_list {
                    display: flex;
                    justify-content: space-between;
                    flex-wrap: wrap;
                    .list-2 {
                        display: none;
                    }
                }
            }
        }
    }
}
</style>