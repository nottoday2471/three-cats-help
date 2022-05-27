<template>
    <div class="v-about" id="about">
        <div class="v-about_page">
            <img src="../assets/pages/About-page.png" alt="about-page">
            <div class="v-about_page_text">
                <p>The collection of three help cats is not about commercial earnings for the author. <br><br>
                    This collection is the first of a series that will appear in the future. 
                    It was created to help shelters for homeless animals in Ukraine.<br><br>

                    Since the current situation in the country has increased the number of homeless animals to 67%, 
                    and every abandoned or lost kitten or puppy needs help and your support.<br><br>

                    Part of the money received from the sale of the collection is immediately sent to shelters across the country. 
                    This can be tracked on the site in the "Reports" tab.<br><br>

                    Those funds that we save are spent on creating a new collection.<br><br>

                    As the author of this project, I am grateful to you for your support and purchase of each NFT.<br><br>
                </p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.v-about {
    background: url('../assets/backgrounds/Cat-paws.png'), #E3FFFA;
    width: 100%;
    display: flex;
    justify-content: center;
    padding: 1rem 0 0 0;
    &_page {
        padding: 1rem;
        position: relative;
        &_text {
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            margin: 6rem 0 0 0;
            width: 90%;
            p {
                margin: 0;
                padding: 0;
                font-size: 1.75rem;
            }
        }
    }
}
</style>