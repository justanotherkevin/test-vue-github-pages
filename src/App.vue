<template>
  <div id="app">
    <img src="./assets/logo.png">
    <ul id='nav-bar'>
      <li><router-link to='/'>home</router-link></li>
      <li><router-link to='/test'>test</router-link></li>
      <li><router-link to='/scraper'>scraper</router-link></li>
    </ul>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
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
#nav-bar {
  list-style: none;
  padding: 0;
}
#nav-bar > * {
  display: inline-block;
  padding: 0 11px;
}
</style>
