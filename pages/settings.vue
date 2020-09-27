<template lang="pug">
  section
    v-card
      v-card-text
        v-simple-table
          template
            thead
              tr
                th Setting
                th Value
            tbody(
              v-for="(setting, index) in settings"
              :key="index"
            )
              setting-item(
                :setting="setting"
                :index="index"
                :changeDark="changeDark"
              )

</template>

<script>
import SettingItem from '../components/layout/SettingItem';

export default {
  components: {SettingItem},
  data() {
    return {
      settings: {
        setDarkMode: {
          settingName: 'Dark mode',
          settingValue: true,
        },
      },
    };
  },
  methods: {
    changeDark: function () {
      this.$vuetify.theme.dark = !this.$vuetify.theme.dark
    }
  }

};
</script>

<style scoped>

</style>
