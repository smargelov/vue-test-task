<template lang="pug"> 
  v-navigation-drawer(
    v-model="drawerLeft"
    app
    clipped
    left
  )
    v-list(dense)
      v-list-item(link)
        v-list-item-action
          v-icon mdi-account-multiple
        v-list-item-content
          v-list-item-title Users

      v-list-item(link)
        v-list-item-action
          v-icon mdi-account-key
        v-list-item-content
          v-list-item-title Groups

</template>
