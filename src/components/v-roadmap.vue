<template>
    <div class="v-roadmap" id="roadmap">
        <div class="v-roadmap_title">
            <img src="../assets/links/Roadmap-title.png" alt="roadmap-title">
            <img src="../assets/links/Roadmap-mobile.png" alt="roadmap-title" class="mobile-roadmap-title">
        </div>
        <div class="v-roadmap_wrapper">
            <div class="v-roadmap_wrapper_content">
                <div class="v-roadmap_wrapper_content_text">
                    <p>1. The first prototype three cat help! NFT was minted.</p>
                    <p>2. Three help cats officially starts at the Polygon! The collection is born.</p>
                    <p>3. Reach a sale of 5.000 NFT art</p>
                    <p>4. Transfer the proceeds from the sale of NFT art to animal shelters.</p>
                    <p>5. Unlock the first manga about Three Helping Cats.</p>
                    <p>6. Launch the second "Three Dogs Help" collection.</p>
                    <p>7. All owners who get 3 or more of NFT "Three Cats Help" can get 1 random NFT from next collection</p>
                    <p class="v-roadmap_wrapper_content_text_secret-text">Something special soon...</p>
                </div>
                <div class="v-roadmap_wrapper_content_picture">
                    <img src="../assets/links/Roadmap-picture2.png" alt="roadmap-title">
                    <img src="../assets/links/Roadmap-picture-mobile.png" alt="roadmap-title" class="roadmap-picture">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.v-roadmap {
    background: url('../assets/backgrounds/Cat-paws-roadmap.png'), #F3E3FF;
    width: 100%;
    min-height: 940px;
    padding: 1rem 0 0 0;
    &_title {
        display: flex;
        justify-content: center;
        .mobile-roadmap-title {
            display: none;
        }
    }
    &_wrapper {
        display: flex;
        justify-content: center;
        padding: 2rem 0 0 0;
        &_content {
            display: flex;
            justify-content: space-between;
            margin: 1rem 0 0 0;
            width: 1300px;
            &_text {
                background: #ffff;
                display: inline-block;
                border: 1px solid black;
                border-radius: 48px;
                padding: 0 1.5rem 1.5rem 1.5rem;
                font-size: 1.25rem;
                p {
                    margin: 3rem 0 0 0;
                    padding: 0;
                }
                &_secret-text {
                    font-size: 2.25rem;
                    font-weight: 700;
                    text-align: center;
                }
            }
            &_picture {
                .roadmap-picture {
                    display: none;
                }
            }
        }
    }
}

@media only screen and (max-width: 1350px) {
    .v-roadmap {
        height: 812px;
        &_title {
            img {
                display: none;
            }
            .mobile-roadmap-title {
                display: block;
            }
        }
        &_wrapper {
            padding: .5rem 0 0 0;
            &_content {
                display: flex;
                justify-content: space-between;
                flex-direction: column;
                margin: 1rem 0 0 0;
                max-width: 350px;
                &_text {
                    font-size: 1rem;
                    p {
                        margin: 1rem 0 0 0;
                        padding: 0;
                    }
                    &_secret-text {
                        font-size: 1.75rem;
                    }
                }
                &_picture {
                    img {
                        display: none;
                    }
                    .roadmap-picture {
                        display: block;
                    }
                }
            }
        }
    }
}

</style>