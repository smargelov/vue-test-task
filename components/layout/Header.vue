<template lang="pug">
  v-app-bar(
    app
    clipped-left
    color="dark"
    dark
  )
    v-app-bar-nav-icon(@click.stop="changeDrawer")
    v-toolbar-title
      n-link(
        class="white--text"
        to="/"
      ) Test task
    v-spacer

</template>

<script>
export default {
  props: ['changeDrawer']
}
</script>

<style lang="sass">

</style>
