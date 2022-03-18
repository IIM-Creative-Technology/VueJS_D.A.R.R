<script setup>
import WellDone from './WellDone.vue'

</script>

<style>
</style>

<template>

    <div id="app1">
        <p>#pond {</p>
        <p>display: flex;</p>
        <textarea v-model="checkedNames" id="text" placeholder="edit me"></textarea>
        <p>}</p>
        <button id="btn" v-on:click="checkForm">Suivant</button>
    </div>



</template>
<script>

export default {
  data() {
    return {
        checkedNames: ''
    }
  },
  methods:{
      checkForm(){
          var input = document.getElementById("text").value;
          console.log(input)
          console.log("formulaire a été bien envoyé !")
          if(input == "salut"){
              console.log("bravo")
          }else{
              console.log("nop")
          }
      },

      
  },
  
}
</script>
