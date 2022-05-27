<template>
    <div class="v-nav-to-content">
        <ul>
            <li>
                <a href="#about">
                    <img src="../assets/links/About.png" alt="about">
                </a>
            </li>
            <li>
                <a href="#roadmap">
                    <img src="../assets/links/Roadmap.png" alt="roadmap">
                </a>
            </li>
            <li>
                <a href="#gallery">
                    <img src="../assets/links/Gallery.png" alt="gallery">
                </a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
.v-nav-to-content {
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