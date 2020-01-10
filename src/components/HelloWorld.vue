<template>
  <div class="hello">
    
    <h2>{{name}}</h2>
    <h1>{{ msg }}</h1>
      <router-link to='/page01'>page01</router-link>
   
  </div>
</template>

<script>
export default {

  data () {
    return {
      name:'HelloWorld',
      msg: 'Hello,Vue'
    }
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
.hello{
  background: #ff3344;
}
</style>
