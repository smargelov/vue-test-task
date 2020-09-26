<template lang="pug">
  v-navigation-drawer(
    v-model="drawerState"
    app
    clipped
    left
  )
    v-list(dense)
      v-list-item(
        to="/users"
        nuxt
      )
        v-list-item-action
          v-icon mdi-account-multiple
        v-list-item-content
          v-list-item-title Users

      v-list-item(
        to="/posts"
        nuxt
      )
        v-list-item-action
          v-icon mdi-account-key
        v-list-item-content
          v-list-item-title Posts

      v-list-item(
        to="/settings"
        nuxt
      )
        v-list-item-action
          v-icon mdi-cog
        v-list-item-content
          v-list-item-title Settings

</template>

<script>
export default {
  props: {
    drawer: {
      type: Boolean,
      default: false
    }
  },
  data() {
    return {
      drawerState: this.drawer
    }
  },
  watch: {
    drawer() {
      this.drawerState = !this.drawerState
    }
  }
}
</script>
