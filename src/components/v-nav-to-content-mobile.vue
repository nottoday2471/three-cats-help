<template>
    <div class="v-nav-to-content-mobile">

        <ul>
            <li>
                <a href="#about">
                    <img src="../assets/links/About-mobile.png" alt="about">
                </a>
            </li>
            <li>
                <a href="#roadmap">
                    <img src="../assets/links/Roadmap-mobile.png" alt="roadmap">
                </a>
            </li>
            <li>
                <a href="#gallery">
                    <img src="../assets/links/Gallery-mobile.png" alt="gallery">
                </a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
.v-nav-to-content-mobile {
    img {
        max-width: 100%;
        height: auto;
    }
    margin: 0 2rem 0 0;
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
                padding: 1rem;
            }
            &:hover {
                opacity: .6;
            }
        }
    }
}
</style>