<template lang="pug">
  v-app-bar(
    app
    clipped-left
    color="dark"
    dark
  )
    v-app-bar-nav-icon(@click.stop="drawerLeft = !drawerLeft")
    v-toolbar-title Test task
    v-spacer

</template>

<script>
export default {

}
</script>

<style lang="sass">

</style>
