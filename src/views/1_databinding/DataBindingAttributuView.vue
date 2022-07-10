<template>
<div>
    <!-- <input type="text" v-bind:value="userId" readonly> -->
    <input type="text" :value="userId" readonly>
    <!-- 속성도 바인딩이 가능함. -->
    <!-- v-bing는 :으로 작성해도가능함. -->
    <br>
    <!-- <img src="" alt="" style="width:100px; height: auto;"> -->
    <!-- 위의 이미지태그를 바인딩하는법 -->
    <img :src="imgsrc" alt="" style="width:100px; height: auto;">
    <br>
    <input type="search" v-model="txt1">
    <button :disabled="txt1===''">조회</button>

</div>

</template>

<script>
export default {
  components() {

  },
  data() {
    return {
      userId: 'parkparkpark',
      imgsrc: 'https://kr.vuejs.org/images/logo.png',
      txt1: ''
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
