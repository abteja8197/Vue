<template>
  <div>
    <h2>Second page</h2>
    <button @click="back">back</button>
    <div>
      <b-table striped hover :items="items"></b-table>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SecondPage',
  methods: {
    back () {
      this.$router.go(-1);
    }
  },
  data() {
      return {
        items: [
          { age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
          { age: 21, first_name: 'Larsen', last_name: 'Shaw' },
          { age: 89, first_name: 'Geneva', last_name: 'Wilson' },
          { age: 38, first_name: 'Jami', last_name: 'Carney' }
        ]
      }
    }
}
</script>