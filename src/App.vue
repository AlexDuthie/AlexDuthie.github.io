<template>
  <main>
    <nav-bar></nav-bar>
    <router-view/>
  </main>
</template>

<script>
import NavBar from './components/NavBar.vue'

export default {
  components: {
    NavBar
  }
}
</script>

<style scoped>
</style>
