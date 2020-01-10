<template>
  <div class="hello">
    hello,
    <div>
      {{msg}}
    </div>
    <div>
      {{time}}
    </div>
  </div>
</template>

<script>
export default {
  /* eslint-disable */
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      time: new Date()
    }
  },
  mounted(){
    setInterval(()=>{this.$data.time=new Date().getTime()},1000)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
