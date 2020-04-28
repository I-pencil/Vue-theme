<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <ThmeeCss />
  </div>
</template>

<script>
// import ThmeeScss from './views/theme-scss'
import ThmeeCss from './views/theme-css-var'

export default {
  name: 'App',
  components: {
    ThmeeCss
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
