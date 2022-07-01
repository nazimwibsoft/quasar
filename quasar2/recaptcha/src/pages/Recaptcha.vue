<template>
  <vue-recaptcha sitekey="6LcmbbgfAAAAAC55miOZbaWqBl8U-ppWIJBvC5L1" @verify="onVerify">
  </vue-recaptcha>

  <q-btn :disabled=!verified color="primary" label="Next" />
</template>

<script>
import { VueRecaptcha } from 'vue-recaptcha'
export default {
  data () {
    return {
      verified: false
    }
  },
  components: { VueRecaptcha },
  methods: {
    onVerify () {
      this.verified = true
      console.log('Verified')
    }
  }
}
</script>
