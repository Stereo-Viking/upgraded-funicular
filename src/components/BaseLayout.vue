<template lang="pug">
  v-app
    BaseAppBar
    v-main
      slot
    BaseFooter
</template>

<script>
import BaseAppBar from "@/components/BaseAppBar"
import BaseFooter from "@/components/BaseFooter"

export default {
  name: "BaseLayout",
  components: {
    BaseAppBar,
    BaseFooter
  },
  props: {
    fluid: {
      type: Boolean,
      default: true
    }
  }
}
</script>