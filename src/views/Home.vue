<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import PayPal from 'vue-paypal-checkout'

export default {
  name: 'home',
  components: {
    HelloWorld,
    PayPal
  },
  data() {
    return {
      paypal: {
        sandbox: 'AXHOQJir4UbLH5hEUbJXJiZiWGV12rNfj_LRPTXbyHe3W7FZfWXKxqoQ3MJv1sY0dsUxi4y9aj7MGqSd',
        production: 'EI7Ueh7U5Yq_H-EgHp62zyUOMNUcIS07Azav3_D-FG41Fq1MrxLlyygiQc5_DWSqomiua8-tAu4cw746'
      }
    }
  }
}
</script>
