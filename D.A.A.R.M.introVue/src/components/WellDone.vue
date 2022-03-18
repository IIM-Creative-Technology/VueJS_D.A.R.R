<template>
    <div id="app">	
        <!-- <p>Random Number = {{randomNumber}}</p> -->
        <p>Random Number = {{formatNumber}}</p>
        <button @click="myFunction()">Click Me</button>
    </div>
</template>
<script>
export default {
  data() {
    return {
        randomNumber:'',
        formatNumber: ''
    }
  },
  methods:{
    myFunction: function () {		
        this.randomNumber = Math.random()*100; 
        this.formatNumber = this.randomNumber.toFixed(0);

        if (this.formatNumber % 2 === 0){
            console.log("Pair")
        }else{
            console.log("Impair")
        }
    }   
   },
  
}
</script>   