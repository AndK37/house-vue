<template>
  <my-header/>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view/>
</template>

<script>
import MyHeader from '@/components/MyHeader.vue'

export default {
 components: {
  "my-header": MyHeader,
 }
}
</script>

<style>
#app {

}
body {
  margin: 0;
  padding: 0;
}


nav a.router-link-exact-active {

}
</style>
