<template>
    <div class="v-header">
        <div class="v-header_logo">
            <div class="v-header_logo_content">
                <img src="../assets/links/logo.png" alt="logo">
            </div>
        </div>
        <div class="v-header_nav-links">
            <v-nav-to-content />
            <v-nav-to-social-media />
        </div>
    </div>
</template>

<script setup>
import VNavToContent from './v-nav-to-content.vue'
import VNavToSocialMedia from './v-nav-to-social-media.vue'

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
    }
    &_nav-links {
        height: 100%;
        display: flex;
        justify-content: center;
    }
}
</style>