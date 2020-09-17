<template lang="pug">
  v-app-bar(
    app
    clipped-left
    color="dark"
    dark
  )
    v-app-bar-nav-icon(@click.stop="drawerLeft = !drawerLeft")
    v-toolbar-title
      n-link(
        class="white--text"
        to="/"
      ) Test task
    v-spacer

</template>

<script>
export default {
  data: () => ({
    drawerLeft: true,
  }),
}
</script>

<style lang="sass">

</style>
