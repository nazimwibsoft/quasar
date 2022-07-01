<template>
  <router-view />
  <VueBrowserUpdate />
</template>
<script>
import { defineComponent } from 'vue'
import VueBrowserUpdate from 'vue-browserupdate'

export default defineComponent({
  name: 'App',
  components: {
    VueBrowserUpdate
  }
})
</script>
