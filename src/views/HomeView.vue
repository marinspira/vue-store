<template>
  <div class="home">
    <Banner/>
    <Menu/>
  </div>
</template>

<script>
import Banner from '@/components/Banner.vue';
import Menu from '@/components/Menu.vue'

export default {
  components: {
    Banner,
    Menu
  }
}
</script>

<style>
.home {
  background-color: var(--color-grey);
}
</style>
