<template>
  <NavBar />
  <router-view></router-view>
</template>

<script>

import NavBar from "/Hoc/Vuejs/hello-world/src/components/Navbar.vue"
export default {
  name: "AppPage",
  components: {
    NavBar
  },
};
</script>

<style></style>