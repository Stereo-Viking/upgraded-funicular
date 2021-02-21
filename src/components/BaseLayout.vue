<template lang="pug">
  v-app
    BaseAppBar
    v-main
      slot
</template>

<script>
import BaseAppBar from "@/components/BaseAppBar"

export default {
  name: "BaseLayout",
  components: {
    BaseAppBar
  },
  props: {
    fluid: {
      type: Boolean,
      default: true
    }
  }
}
</script>