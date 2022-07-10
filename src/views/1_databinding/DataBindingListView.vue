<template>
<div>
    <select name="" id="">
        <option value=""></option>
        <option :value="city.code" :key="city.code" v-for="city in cities">{{city.title}}</option>
    </select>
<div>
    <table>
        <thead>
            <tr>
                <th>제품번호</th>
                <th>제품명</th>
                <th>가격</th>
                <th>주문수량</th>
                <th>합계</th>
            </tr>
        </thead>
        <tbody>
            <tr :key="drink.drinkid" v-for="drink in drinklist">
                <td>{{drink.drinkid}}</td>
                <td>{{drink.drinkName}}</td>
                <td>{{drink.price}}</td>
                <td>{{drink.qty}}</td>
                <td><input type="number" v-model="drink.qty"></td>
                <td>{{drink.price*drink.qty}}</td>
            </tr>
        </tbody>
    </table>
</div>
</div>

</template>

<script>
export default {
  components() {

  },
  data() {
    return {
      cities: [
        { title: '서울', code: '02' },
        { title: '부산', code: '051' },
        { title: '제주', code: '064' }
      ],
      drinklist: [
        {
          drinkid: '1',
          drinkName: '코카콜라',
          price: 1000,
          qty: 1
        },
        {
          drinkid: '2',
          drinkName: '사이다',
          price: 2000,
          qty: 11
        },
        {
          drinkid: '3',
          drinkName: '제주감귤',
          price: 3000,
          qty: 21
        }
      ]
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
