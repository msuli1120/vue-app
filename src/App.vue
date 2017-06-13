<template>
  <div>
    <app-header></app-header>
    <vue-app></vue-app>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Vueapp from './components/Vueapp.vue'
export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'vue-app': Vueapp,
  },
  data () {
    return {
      title: 'Vue App'
    }
  }
}
</script>

<style scoped>
h1 {
  color: purple;
}
</style>
