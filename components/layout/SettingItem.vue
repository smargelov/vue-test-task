<template lang="pug">
  tr
    td {{setting.settingName}}
    td
      v-switch(
        v-model="setting.settingValue"
        @change="changeDark"
      )

</template>

<script>
export default {
  props: [
    'setting',
    'index',
    'changeDark'
  ],


};
</script>

<style scoped>

</style>
