<template>
  <div class="electronics">
    <HelloWorld msg="electronics" :items="items"/>
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Electronics',
  components: {
    HelloWorld
  },
  data () {
    return {
      items: ['電子零組件業', '電子通路業','其他電子業']
    }
  }
}
</script>
