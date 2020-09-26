<template  lang="pug">
  section
    v-card
      v-card-text
        v-simple-table
          template(v-slot:default)
            thead
              tr
                th #
                th Setting
                th Value
            tbody
              tr
                td 1
                td Set dark mode
                td
                  v-switch(
                    v-model="isDark"
                  )
</template>

<script>
export default {
data () {
  return {
    isDark: true,
  }
}

};
</script>

<style scoped>

</style>
