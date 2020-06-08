<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App" :items="todayItems"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  },
  data () {
    return {
      items: [ '水泥工業','塑膠工業','航運業','電機機械','電器電纜','觀光事業','貿易百貨業','食品工業','紡織纖維','橡膠工業','半導體業','光電業','通信網路業','資訊服務業','電腦及週邊設備業','生技醫療業','化學工業','玻璃陶瓷','造紙工業','鋼鐵工業','汽車工業','建材營造業','其他業','油電燃氣業','電子商務','文化創意業','農業科技業'],
      todayItems: []
    }
  },
  created() {
    const randomItem = this.randomItem()
    this.todayItems = [randomItem]
  },
  methods: {
    randomItem () {
      const randomItem = this.items[Math.floor(Math.random() * this.items.length)];
      return randomItem
    }
  }

}
</script>
