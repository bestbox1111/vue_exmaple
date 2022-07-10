<template>
<div>
    <button @click="increaseCounter">Add 1</button>
    <h1>{{counter}}</h1>
</div>

</template>

<script>
export default {
  components() {

  },
  data() {
    return {
      counter: 0
    }
  },
  setup() {

  },
  created() {

  },
  mounted() {

  },
  unmounted() {

  },
  methods: {
    increaseCounter() {
      this.counter += 1
    }
  }
}
</script>

<style scoped>

</style>
