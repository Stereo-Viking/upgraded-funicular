<template lang="pug">
  v-footer(
    app
    absolute
    padless
    inset
  ): v-container(fluid).pa-0.ma-0
    v-row(
      justify="center"
      no-gutters
    )
      v-card(
        flat
        tile
      ).ligten-1.text-center
        v-card-text
          v-row: IconsSocial
          v-row(
            justify="center"
            no-gutters
          ).pt-2
            span.text-center {{ year }} - <strong>Stereo Viking</strong>
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