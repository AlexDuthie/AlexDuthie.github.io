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

<style>
main {
  height: 100%;
  width: 100%;
  background-color: #eee;
}
</style>
