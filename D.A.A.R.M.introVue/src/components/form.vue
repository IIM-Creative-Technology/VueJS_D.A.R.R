<template>
    <div id="app">	
        <!-- <p>Random Number = {{randomNumber}}</p> -->
        <p>Random Number = {{count}}</p>
        <button @click="myFunction()">Click Me</button>
        <img src="https://store-images.s-microsoft.com/image/apps.51232.14176082463109974.f84fc39e-bc64-44f3-9851-edbbe1a9d810.d3b66324-8c44-4ac1-8df3-fc47485eb9f0?mode=scale&q=90&h=1080&w=1920" v-if="count == 1" alt="">
        <img src="https://static.posters.cz/image/750/affiches-et-posters/beach-sunset-i102003.jpg" v-if="count == 2" alt="">
        <button @click="reload()">Refresh</button>

    </div>
</template>
<style>
img{
    width: 100px;
    height: 100px;
}
</style>
<script>
export default {
  data() {
    return {
        count : 0,
    }
  },
  methods:{
    myFunction: function () {		
        this.count = this.count + 1; 
    },
    reload: function () {		
        this.count = 0;
    }    
   },
  
}
</script>   