<template>
<div>
    <div>
        <input type="radio" id="html" value="html" v-model="lang">
        <label for="html">html</label>
    </div>
    <div>
        <input type="radio" id="css" value="css"  v-model="lang">
        <label for="css">css</label>
    </div>
    <div>
        <input type="radio" id="js" value="js"  v-model="lang">
        <label for="js">js</label>
    </div>
<div>
선택한 지역 : {{lang}}
</div>
</div>

</template>

<script>
export default {
  components() {

  },
  data() {
    return {
      lang: ''
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

  }
}
</script>

<style scoped>

</style>
