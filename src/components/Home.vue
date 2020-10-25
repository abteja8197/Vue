<template>
  <div>
    <h1>Home</h1>
    <button @click="firstOne">First</button>
    <button @click="secondOne">Second</button>
    <router-view></router-view>
  </div>
</template>
<script>
export default {
  name: 'Home',
  methods: {
    firstOne () {
      this.$router.push({ name: 'FirstPage' })
    },
    secondOne () {
      this.$router.push({name: 'SecondPage'})
    }
  }
}
</script>