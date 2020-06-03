<template>
  <div class="hello">
    <vue-tabs>
        <v-tab title="First tab">
          First tab content
        </v-tab>

        <v-tab title="Second tab">
          Second tab content
        </v-tab>

        <v-tab title="Third tab">
          Third tab content
        </v-tab>
    </vue-tabs>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
