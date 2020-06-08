<template>
  <div class="etf">
    <HelloWorld msg="etf" :items="items"/>
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'ETF',
  components: {
    HelloWorld
  },
  data () {
    return {
      items: [ 'ETF']
    }
  }
}
</script>
