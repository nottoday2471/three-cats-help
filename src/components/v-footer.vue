<template>
    <div class="v-footer">
        <div class="v-footer_text">
            <p>Three cats help / CryptoDon 2022</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.v-footer {
    width: 100%;
    height: 55px;
    background: #FFB47D;
    border-top: 1px solid black;
    display: flex;
    justify-content: center;
    flex-direction: column;
    &_text {
        display: flex;
        justify-content: center;
        p {
            margin: 0;
            padding: 0;
            display: inline-block;
            font-size: 1.75rem;
            font-weight: 700;
        }
    }
}

@media only screen and (max-width: 428px) {
    .v-footer {
        &_text {
            p {
                font-size: 1.25rem;
            }
        }
    }
}
</style>