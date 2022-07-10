<template>
<div>
    <!-- template아래에 최상위 html태그가 하나는 필요히여 div필요.  -->
    <h1>Hellow ~~ !!! {{userName}}</h1>
    <p>{{message}}</p>
</div>

</template>

<script>
export default {
  data() {
    return {
      // 데이터 바인딩시 스트링
      userName: 'park jun hyung',
      message: 'Welcome 개발자의 품격',
      // 배열
      arr: [],
      // 오브제에 따라 다 라우터시키는 방법이 다른듯.
      obj: {}
    }
  }
}
</script>

<style scoped>
/* scoped적용하면 지역변수처럼 이 컴퍼넌트에만 스타일 적용됨. */
.text-red{
    color:red;
}

</style>
