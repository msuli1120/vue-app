<template>
  <div id="apps">
    <ul>
      <li v-for="app in apps" @click="app.show = !app.show">
        <h2>{{ app.name }}</h2>
        <h3 v-show="app.show">{{ app.speciality }}</h3>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    data(){
      return {
        apps: [
          {name: 'Max', speciality: 'Vue Components', show: false},
          {name: 'Mario', speciality: 'HTML Wizardry', show: false},
          {name: 'Matt', speciality: 'Click Events', show: false},
          {name: 'Tango', speciality: 'Conditionals', show: false},
          {name: 'Rob', speciality: 'Webpack', show: false},
          {name: 'Xing', speciality: 'Data Diggin', show: false}
        ]
      }
    }
  }
</script>

<style scoped>
  #apps {
    width: 100%;
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
    box-sizing: border-box;
  }
  ul {
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
  }
  li {
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 1px solid #222;
    margin: 10px;
  }
</style>
