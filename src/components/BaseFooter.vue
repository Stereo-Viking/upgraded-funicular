<template lang="pug">
  v-footer(
    app
    absolute
    padless
    inset
  )
    v-spacer
    v-row(
      justify="center"
      no-gutters
    )
      v-card(
        flat
        tile
        color="transparent"
      ).text-center
        v-card-text
          v-row: IconsSocial
          v-row(
            justify="center"
          ).pt-2
            span.text-center {{ year }} - <strong>Stereo Viking</strong>
      v-spacer
</template>

<script>
import IconsSocial from "@/components/IconsSocial"

export default {
  name: "BaseFooter",
  components: {
    IconsSocial
  },
  computed: {
    year: function() {
      return new Date().getFullYear()
    }
  }
}
</script>