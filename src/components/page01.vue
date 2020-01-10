<template>
  <div id="rzh">
      
     
      <h1>{{ msg }}</h1>
        <input type="text" v-model="model">
        <div>{{ model }}</div>
        <h1 v-if="yes">你看到我了</h1>
        <h1 v-else>我藏起来了</h1>
        <button v-on:click="View" >点击隐藏</button>
        <h2>--------------------分割线--------------------</h2>
        <h1 v-show="show">我是V-show</h1>
      
        <ul v-for="item in vm" :key="item.id">
          <li>{{ item.name }}</li>
          <li>{{ item.age }}</li>
        
        </ul>
       
        <router-link to = '/'>返回首页</router-link>

  </div>
</template>

<script>
export default {

data:function(){

  
      return{   
                  vm : [{
              name:'Jack',
              age:'20'
            },
            {
            name:'Rose',
            age:'18'
            },
            {
              name:'titanic',
              age:'3'
            }
            ],
            yes:true,
           show:true,
             msg:'我是daddy',
            model:'IM model'
  }
},
methods:{

 
    View() {
     
     
      this.yes = !this.yes
     this.show = !this.show
      //  console.log(this.yes)
    }
}
}
</script>

<style>
#rzh{
    background: yellow;
}
h1{
    color: aqua;
}
</style>