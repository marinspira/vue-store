<template>
    <div class="main-container">
        <ul class="menu">
            <li>
                <img :src="menu1" alt="" id="menu-img">
                <div>
                    <p>Novos Dragons</p>
                    <button>Pedir agora</button>
                </div>
            </li>
            <li>
                <img :src="menu2" alt="" id="menu-img">
                <div>
                    <p>King Jr</p>
                    <button>Pedir agora</button>
                </div>
            </li>
            <li>
                <img :src="menu3" alt="" id="menu-img">
                <div>
                    <p>Queen Cheese</p>
                    <span></span>
                    <button>Pedir agora</button>
                </div>
            </li>
            <li>
                <img :src="menu4" alt="" id="menu-img">
                <div>
                    <p>Whopper e CBK</p>
                    <span></span>
                    <button>Pedir agora</button>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "Menu",
    data() {
        return {
            menu1: '/img/menu1.webp',
            menu2: '/img/menu2.webp',
            menu3: '/img/menu3.webp',
            menu4: '/img/menu4.webp'
        }
    }
}
</script>

<style scoped>
    .menu {
        max-width: 100%;
        display: flex;
        margin-top: 150px;
        padding-left: 0;
        flex-wrap: wrap;
    }

    .menu img {
        width: 100%;
    }

    .menu li {
        padding: 20px 10px;
        width: 50%;
    }

    .menu p {
        font-family: Flame, "Cooper Black", "Helvetica Neue", Helvetica, Arial, sans-serif;
        font-size: 23px;
    }

    .menu li div {
        background-color: var(--color-brow);
        display: flex;
        justify-content: space-between;
        padding: 15px 20px;
        border-radius: 0px 0 10px 10px;
        color: var(--color-grey);
        align-items: center;
    }
</style>