<template>
    <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/" class="logo_url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <router-link to="/pedidos">Pedidos</router-link>
    </nav>
</template>

<script>
export default {
    name: "Navbar",
    props: ["logo", "alt"]
}
</script>

<style scoped>
    nav {
        position: relative;
        display: flex;
        justify-content: space-between;
        background: var(--color-grey);
        color: rgb(31, 31, 31);
        height: 78px;
        margin-block: 0px;
        margin-inline: auto;
        padding: 10px 30px;
        width: 100%;
        align-items: center;
        box-shadow: rgba(0, 0, 0, 0.1) 0px 1px 1px;
    }

    #logo, .logo_url {
        height: 100%;
    }

    a {
        color: var(--color-brow);
        font-family: Flame, "Cooper Black", "Helvetica Neue", Helvetica, Arial, sans-serif;
        font-size: 20px;
    }
</style>