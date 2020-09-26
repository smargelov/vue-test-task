<template lang="pug">
  section
    v-card
      v-card-text
        v-simple-table
          template
            thead
              tr
                th #
                th Setting
                th Value
            tbody(
              v-for="(setting, index) in settings"
              :key="index"
            )
              setting-item(
                :setting="setting"
                :index="index"
              )

</template>

<script>
import SettingItem from '../components/layout/settingItem';

export default {
  components: {SettingItem},
  data() {
    return {
      settings: [
        {
          settingName: 'Set dark mode',
          settingValue: true
        }
      ]
    };
  },

};
</script>

<style scoped>

</style>
