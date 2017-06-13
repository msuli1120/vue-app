<template>
  <div>
    <h1>{{ title }}</h1>
    <vueapp></vueapp>
  </div>
</template>

<script>
import Vueapp from './Vueapp.vue'

export default {
  components: {
    'vueapp': Vueapp,
  },
  data () {
    return {
      title: 'Vue App'
    }
  }
}
</script>

<style>

</style>
