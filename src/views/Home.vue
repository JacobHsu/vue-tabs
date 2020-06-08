<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App" :items="items"/>
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
      items: [ '航運業','觀光事業','貿易百貨業','食品工業','紡織纖維','橡膠工業','半導體業','光電業','通信網路業','資訊服務業','電腦及週邊設備業','電子通路業']
    }
  }
}
</script>
