<template lang="pug">
  v-parallax(:src="image")
    .overlay.d-flex
      slot
</template>

<script>
export default {
  name: 'BaseParallax',
  props: ['image']
}
</script>

<style scoped>
.overlay {
    z-index: 1;
    height: 100%;
    width: 100%;
    position: absolute;
    overflow: hidden;
    top: 0px;
    left: 0px;
    background: rgba(0, 0, 0, 0.75); /*can be anything, of course*/
}
</style>
