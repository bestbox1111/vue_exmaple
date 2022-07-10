<template>
<div>
    <select name="" id="" @change="changeCity" v-model="selectedCity">
        <option value="">==도시 선택==</option>
        <option :value="city.cityCode" :key="city.cityCode" v-for="city in cityList">{{city.title}}</option>

    </select>
    <select name="" id="">
        <option value="dong.dongCode" :key="dong.dongCode" v-for="dong in selectedDongList">{{dong.dongTitle}}</option>
    </select>
</div>
</template>

<script>
export default {
  components() {

  },
  data() {
    return {
      selectedCity: '',
      cityList: [
        { title: '서울', cityCode: '02' },
        { title: '부산', cityCode: '051' },
        { title: '제주', cityCode: '064' }
      ],
      dongList: [
        { dongTitle: '서울1동', dongCode: '1', cityCode: '02' },
        { dongTitle: '서울2동', dongCode: '2', cityCode: '02' },
        { dongTitle: '서울3동', dongCode: '3', cityCode: '02' },
        { dongTitle: '서울4동', dongCode: '4', cityCode: '02' },
        { dongTitle: '부산1동', dongCode: '1', cityCode: '051' },
        { dongTitle: '브신2동', dongCode: '2', cityCode: '051' },
        { dongTitle: '부산3동', dongCode: '3', cityCode: '051' },
        { dongTitle: '부산4동', dongCode: '4', cityCode: '051' },
        { dongTitle: '제주1동', dongCode: '1', cityCode: '064' },
        { dongTitle: '제주22동', dongCode: '2', cityCode: '064' },
        { dongTitle: '제주3동', dongCode: '3', cityCode: '064' },
        { dongTitle: '제주4동', dongCode: '4', cityCode: '064' }
      ],
      selectedDongList: []
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
    changeCity() {
      this.selectedDongList = this.dongList.filter(dong => dong.cityCode === this.selectedCity)
    }
  }
}
</script>

<style scoped>

</style>
