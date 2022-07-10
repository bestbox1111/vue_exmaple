<template>
    <div>
        <!-- 아래 단락은 {{}}으로 인해 그냥 문자열로 전달될뿐. -->
        <div>{{htmlString}}</div>
        <!-- 아래와 같이 v-html로 적용해야 inerhtml로 적용됨. -->
        <div v-html="htmlString"></div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      htmlString: '<p style="color:red;">빨간색</p>'
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
