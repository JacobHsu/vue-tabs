<template>
  <div class="financial">
    <HelloWorld msg="financial" :items="items"/>
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Financial',
  components: {
    HelloWorld
  },
  data () {
    return {
      items: [ '金控業','銀行業','證券業','保險業']
    }
  }
}
</script>
