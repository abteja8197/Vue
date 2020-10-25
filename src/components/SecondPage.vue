<template>
  <div>
    <h2>
      Second page
    </h2>
    <button @click="back">back</button>
  </div>
</template>

<script>
export default {
  name: 'SecondPage',
  methods: {
    back () {
      this.$router.go(-1);
    }
  }
}
</script>