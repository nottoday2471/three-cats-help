<template>
    <div class="v-nav-to-social-media">
        <div class="v-nav-to-social-media_list">
            <div class="v-nav-to-social-media_list_item">
                <a href="https://www.instagram.com/ruslan_konoshenko/" target="_blank">
                    <img src="../assets/links/Instagram.png" alt="instagram">
                </a>
            </div>
            <div class="v-nav-to-social-media_list_item">
                <a href="https://discord.gg/SQ4WGdxZ" target="_blank">
                    <img src="../assets/links/Discord.png" alt="discord">
                </a>
            </div>
            <div class="v-nav-to-social-media_list_item">
                <a href="https://twitter.com/RuslanKonoshenk" target="_blank">
                    <img src="../assets/links/Twitter.png" alt="twitter">
                </a>
            </div>
            <div class="v-nav-to-social-media_list_item">
                <a href="https://opensea.io/collection/three-cats-help" target="_blank">
                    <img src="../assets/links/Opensea.png" alt="opensea">
                </a>
            </div>
            <div class="v-nav-to-social-media_list_item">
                <a href="https://www.youtube.com/channel/UC6Y35yrm6_WoX5FyS6sr5KQ" target="_blank">
                    <img src="../assets/links/Youtube.png" alt="youtube">
                </a>
            </div>
            <div class="v-nav-to-social-media_list_item">
                <a href="https://t.me/crypt_don" target="_blank">
                    <img src="../assets/links/Telegram.png" alt="telegram">
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.v-nav-to-social-media {
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