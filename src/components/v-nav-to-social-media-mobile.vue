<template>
    <div class="v-nav-to-social-media-mobile">
        <ul>
            <li>
                <a href="https://www.instagram.com/ruslan_konoshenko/">
                    <img src="../assets/links/Instagram-mobile.png" alt="instagram">
                </a>
            </li>
            <li>
                <a href="#" target="_blank">
                    <img src="../assets/links/Discord-mobile.png" alt="discord">
                </a>
            </li>
            <li>
                <a href="https://twitter.com/RuslanKonoshenk" target="_blank">
                    <img src="../assets/links/Twitter-mobile.png" alt="twitter">
                </a>
            </li>
            <li>
                <a href="https://opensea.io/collection/three-cats-help" target="_blank">
                    <img src="../assets/links/Opensea-mobile.png" alt="opensea">
                </a>
            </li>
            <li>
                <a href="https://www.youtube.com/channel/UC6Y35yrm6_WoX5FyS6sr5KQ" target="_blank">
                    <img src="../assets/links/Youtube-mobile.png" alt="youtube">
                </a>
            </li>
            <li>
                <a href="https://t.me/crypt_don" target="_blank">
                    <img src="../assets/links/Telegram-mobile.png" alt="telegram">
                </a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
.v-nav-to-social-media-mobile {
    display: flex;
    justify-content: center;
    flex-direction: column;
    ul {
        margin: 0;
        padding: 0;
        list-style-type: none;
        overflow: hidden;
        li {
            float: left;
            a {
                padding: .5rem;
            }
            &:hover {
                opacity: .6;
            }
        }
    }

}
</style>