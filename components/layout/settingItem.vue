<template lang="pug">
  tr
    td {{index + 1}}
    td {{setting.settingName}}
    td
      v-switch(
        v-model="setting.settingValue"
      )

</template>

<script>
export default {
  props: [
    'setting',
    'index'
  ],


};
</script>

<style scoped>

</style>
