<template lang="pug">
  BaseLayout
    v-container(fluid).d-flex.justify-center
      v-card(
        max-width="400"
        flat
      ).logo
        v-img(alt="Viking Logo" src="@/assets/logo.svg")
        h1 STEREO VIKING
</template>

<script>
import BaseLayout from "@/components/BaseLayout"

export default {
  name: "Home",
  components: {
    BaseLayout
  }    
}
</script>

<style>
.logo {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

