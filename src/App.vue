<template>
  <div id="app">
    <img src="./assets/logo.png" />
    <nav>
      <router-link v-bind:to="{ name: 'Home' }" class>Home</router-link>
      <router-link v-bind:to="{ name: 'FirstPage' }" class>FirstPage</router-link>
      <router-link v-bind:to="{ name: 'SecondPage' }" class>SecondPage</router-link>
    </nav>
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App'
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
