<template lang="pug">
  v-app-bar(
    app
    clipped-left
  )
    v-spacer
    v-card(
      color="transparent"
      tile
      flat
    ).d-flex
      v-img(
        contain
        alt="Stereo Viking Logo"
        width=50
        transition="scale-transition"
        src="@/assets/logo.svg"
        hide-on-scroll
      ).pa-4
    v-spacer
</template>

<script>
export default {
    name: 'BaseAppBar'
}
</script>