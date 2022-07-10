<template>
    <div>
      <!-- v-model=양방향 데이터모델 -->
        <input type="text" v-model="userId">
        <button @click="myfunction">클릭</button>
        <button @click="change">변경</button>
        <br>
        <br>
        <!-- 아래와 같이 작업하면 스트링으로 계산이된다. -->
        <input type="text" v-model="num1"/> +
        <input type="text" v-model="num2"/> =
        <span>{{num1+num2}}</span>
        <br>
        <br>
        <input type="text" v-model.number="num3"/> +
        <input type="text" v-model.number="num4"/> =
        <span>{{num3+num4}}</span>

   </div>
</template>

<script>
export default {
  data() {
    return {
      userId: 'park-jun-hyung',
      num1: 0,
      num2: 0,
      num3: 0,
      num4: 0
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
    // 오브젝트의 특정 키값에 접근하려면 this 키워드를 사용해야함.
    myfunction() {
      console.log(this.userId)
    },
    change() {
      this.userId = "i'am groot"
    }
  }
}
</script>
