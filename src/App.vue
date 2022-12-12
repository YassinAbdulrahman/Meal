<template>
  <div id="app">
    <appheader/>
    <router-view/>
    <app-footer />
  </div>
</template>

<script>
import appheader from "@/components/global/AppHeader.vue";
import AppFooter from "./components/global/AppFooter.vue";
export default {
  components: {
    appheader,
    AppFooter,
  },
};
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
