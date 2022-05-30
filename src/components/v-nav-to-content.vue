<template>
    <div class="v-nav-to-content">
        <div class="v-nav-to-content_list">
            <div class="v-nav-to-content_list_item">
                <a href="#about">
                    <img src="../assets/links/About.png" alt="about">
                </a>
            </div>
            <div class="v-nav-to-content_list_item">
                <a href="#roadmap">
                    <img src="../assets/links/Roadmap.png" alt="roadmap">
                </a>
            </div>
            <div class="v-nav-to-content_list_item">
                <a href="#gallery">
                    <img src="../assets/links/Gallery.png" alt="gallery">
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.v-nav-to-content {
    margin: 0 2rem 0 0;
    display: flex;
    justify-content: center;
    flex-direction: column;
    img {
        max-width: 100%;
        height: auto;
    }
    &_list {
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: space-between;
        &_item {
            padding: .5rem;
            &:hover {
                opacity: .6;
            }
        }
    }
}
</style>