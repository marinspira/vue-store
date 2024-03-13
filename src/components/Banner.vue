<template>
    <div class="banner">
        <div class="main-container">
            <div>
                <h1>O que te apetece hoje?</h1>
                <p>Peça agora e receba em casa!</p>
                <button>Peça agora</button>
            </div>
            <img :src="banner_img" alt="" id="banner">
        </div>
    </div>
</template>

<script>
export default {
    name: "Banner",
    data() {
        return {
            banner_img: "/img/cover.webp"
        }
    }
}
</script>

<style scoped>
    .banner {
        background-color: var(--color-brow);
        height: 200px;
        padding-top: 35px;
    }

    h1, p {
        font-family: Flame, "Cooper Black", "Helvetica Neue", Helvetica, Arial, sans-serif;
        color: var(--color-grey);
    }

    h1 {
        font-size: 52px;
    }

    p {
        font-size: 26px;
        margin: 5px 0 40px 0;
    }

    img {
        height: 275px;
    }


</style>