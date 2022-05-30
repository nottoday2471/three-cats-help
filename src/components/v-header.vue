<template>
    <div class="v-header">
        <div class="v-header_logo">
            <div class="v-header_logo_content">
                <img src="../assets/links/logo.png" alt="logo">
                <img src="../assets/links/Three-cats-help-paw-mobile.png" alt="mobile-logo" class="mobile-logo">
            </div>
        </div>
        <div class="v-header_nav-links">
            <v-nav-to-content />
            <v-nav-to-social-media />
        </div>
        <div class="v-header_nav-links-mobile">
<!--            <v-nav-to-content-mobile />-->
            <v-nav-to-social-media-mobile />
        </div>
    </div>
</template>

<script setup>
import VNavToContent from './v-nav-to-content.vue'
import VNavToSocialMedia from './v-nav-to-social-media.vue'
// import VNavToContentMobile from '@/components/v-nav-to-content-mobile'
import VNavToSocialMediaMobile from './v-nav-to-social-media-mobile'


</script>

<style lang="scss" scoped>
.v-header {
    width: 100%;
    height: 110px;
    background: #FFB47D;
    display: flex;
    justify-content: space-between;
    border-bottom: 1px solid black;
    &_logo {
        margin: 0 0 0 1rem;
        height: 100%;
        display: flex;
        justify-content: center;
        flex-direction: column;
        &_content {
            img {
                max-width: 100%;
                height: auto;
            }
            .mobile-logo {
                display: none;
            }
        }
    }
    &_nav-links {
        height: 100%;
        display: flex;
        justify-content: center;
    }
    &_nav-links-mobile {
        display: none;
        height: 100%;
        justify-content: center;
    }
}

@media only screen and (max-width: 428px) {
    .v-header {
        height: 45px;
        &_logo {
            &_content {
                img {
                    display: none;
                }
                .mobile-logo {
                    display: block;
                }
            }
        }
        &_nav-links {
            display: none;
        }
        &_nav-links-mobile {
            display: flex;
        }
    }
}
</style>