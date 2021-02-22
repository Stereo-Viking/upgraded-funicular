<template lang="pug">
  .icons
    v-btn(
      v-for="(link, icon) in icons"
      :key="icon"
      icon
      :href='link'
    ).mx-3
      v-icon(
        size="24px"
        color="blue"
      ) {{ icon }}
</template>

<script>
export default {
  name: "IconsSocial",
  data: () => ({
    icons: {
      'mdi-facebook': 'https://www.facebook.com/StereoViking',
      'mdi-twitter': 'https://twitter.com/StereoViking',
      'mdi-linkedin': 'https://www.linkedin.com/company/stereoviking/',
    }
  }),
}
</script>