<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <input-form :ttl="title" />
  </div>
</template>

<script>
import InputForm from './components/inputForm.vue'

export default {
  name: 'app',
  components: {
    InputForm
  },
  data(){
    return {
      title: "出席管理"
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
