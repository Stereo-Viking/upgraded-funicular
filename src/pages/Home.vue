<template lang="pug">
  BaseLayout
    BaseParallax(:image='require("@/assets/hero.jpg")')
      v-row(
        align="center"
        justify="center"
      )
        v-col(cols="12").text-center
          h1.display-1.font-weight-thin.mb-4
            | Stereo Viking
          h4.subheading
            | Consumer Purchasing Extinction
</template>

<script>
import BaseLayout from "@/components/BaseLayout"
import BaseParallax from "@/components/BaseParallax"

export default {
  name: "Home",
  components: {
    BaseLayout,
    BaseParallax
  }
}
</script>
