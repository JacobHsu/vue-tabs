<template>
  <div class="hello">
    <vue-tabs>
        <v-tab title="First tab">
          First tab content
          <div class="act-form">
              <iframe :src="src" class="iframe-position"></iframe>
          </div>
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
  },
  data () {
    return {
      src: 'https://segmentfault.com/a/1190000016258735'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.act-form {
  overflow: hidden;
}
.iframe-position {
  width: 900px;
  height: 700px;
  position: relative; 
  top: -310px;
}
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
