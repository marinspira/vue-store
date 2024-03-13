<template>
  <Navbar :logo="logo_src" :alt="app_name"/>
  <router-view/>
</template>

<script>
import Navbar from './components/Navbar.vue'

export default {
  components: {
    Navbar
  },
  data() {
    return {
      logo_src: "/img/logo.webp",
      app_name: "Burger King"
    }
  }
}
</script>

<style>
* {
  margin: 0;
  border: 0;
  box-sizing: border-box;
}

:root {
  --color-brow: rgb(80, 35, 20);
  --color-grey: rgb(245, 235, 220);
  --color-red: rgb(214, 35, 0);
}

a {
  text-decoration: none;
}

button {
  background-color: var(--color-red);
  padding: 15px 100px;
  font-family: Flame, "Cooper Black", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 22px;
  color: var(--color-grey);
  border-radius: 999px;
}

.main-container {
  width: 1200px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin: auto;
}

</style>
