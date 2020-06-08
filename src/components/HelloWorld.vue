<template>
  <div class="hello">
    <vue-tabs>
        <v-tab :title="item" v-for="(item, index) in items" :key="index">
          <div class="act-form">
              <iframe :src="stockList(item)" class="iframe-position"></iframe>
          </div>
        </v-tab>
    </vue-tabs>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    items: Array,
    msg: String
  },
  methods: {
    stockList: function(val) {
      return `https://goodinfo.tw/StockInfo/StockList.asp?MARKET_CAT=全部&INDUSTRY_CAT=${val}&SHEET=交易狀況&SHEET2=日&RPT_TIME=最新資料`
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
  width: 1100px;
  height: 1700px;
  position: relative; 
  top: -940px;
  /* left: -200px; */
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
