<template>
  <div>
    <h1>List of names</h1>
    <ul>
      <li v-for="name in names">{{ name }}</li>
    </ul>
  </div>

</template>

<script>
export default {
  data () {
    return {
      names: ['Mario', 'Max']
    }
  }
}
</script>

<style scoped>
  h1{
    color: green;
  }
</style>
