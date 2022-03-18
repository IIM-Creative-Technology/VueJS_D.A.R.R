<script setup>
import HeaderVue from './components/nav-1.vue'
import Chapter0Vue from './components/Chapter0.vue'
import Chapter1Vue from './components/Chapitre1/Chapter1.vue'
import Chapter2Vue from './components/Chapitre2/Chapter2.vue'
import Chapter3Vue from './components/Chapter3.vue'
import Chapter4Vue from './components/Chapter4.vue'
import Chapter5Vue from './components/Chapter5.vue'
import page5Vue from './components/Chapitre1/pages/page5.vue'



</script>



<template>
<HeaderVue></HeaderVue> 
<section class="left-bar">
  <h4 class="ch" v-on:click="count = 1">Chapitre 1</h4>
  <span class="Chapter1Gr"></span>
  <h4 class="ch" v-on:click="count = 2">Chapitre 2</h4>
  <span class="Chapter2Gr"></span>
  <h4 class="ch" v-on:click="count = 3">Chapitre 3</h4>
  <span class="Chapter3Gr"></span>
  <h4 class="ch" v-on:click="count = 4">Chapitre 4</h4>
  <span class="Chapter4Gr"></span>
  <h4 class="ch" v-on:click="count = 5">Chapitre 5</h4>
  <span class="Chapter5Gr"></span>
</section>
<section class="main">
  <h1>Chapter {{count}}</h1>
  <div class="content">
    <Chapter1Vue v-if="count == 1"></Chapter1Vue> 
    <Chapter2Vue v-if="count == 2"></Chapter2Vue> 
    <Chapter3Vue v-if="count == 3" ></Chapter3Vue> 
    <Chapter4Vue v-if="count == 4"></Chapter4Vue> 
    <Chapter5Vue v-if="count == 5"></Chapter5Vue> 
  </div>
  
</section>
</template>

<script>


export default {
  data(){
    return{
      count: 0
    }
  },
  methods:{
    nextChapter(){
      console.log(this.count)
    }
  },
  
  
}
</script>

<style>
body {
  font-family: poppins;
  margin: 0;
  padding: 0;
}

.main {
  width: 30%;
  height: 782px;
  margin: 0 auto;
  margin-top: -90px;
  background-color: #E4E4E4;
  display: flex;
  justify-self: center;
  align-items: center;
  flex-direction: column;
  border-radius: 65px;
  position: relative;
}

.content{
  display: flex;
  justify-self: center;
  align-content: center;
  flex-direction: column;
  width: 100%;
  height: 80%;
}


.btn-next {
  width: 80px;
  height: 72px;
  border: none;
  background : none;
  cursor: pointer;
  margin-right: 20px;
}

.btn-next:hover{
  background : none;
}

.btn-next > img{
  width: 100%;
  height: 100%;
}

.btn-before {
  width: 80px;
  height: 72px;
  border: none;
  background : none;
  cursor: pointer;
  margin-right: 20px;
}

.btn-before:hover{
  background : none;
}

.btn-before > img{
  width: 100%;
  height: 100%;
  transform: rotate(180deg);
}

.counter{
  font-weight: 900;
  font-size: 48px;
  text-align: center;
  color: #000000;  
  margin: 0;
  margin-left: 20px;
}

.left-bar{
  width: 20%;
  height: 500px;
  position: absolute;
  margin-left: 10%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-size: 25px;
}

.left-bar> span{
  opacity : 1;
  width: 100%;
  height: 2px;
  border-radius:2px solid black;

}

.left-bar >h4:hover {
  border-bottom: 2px solid;
  border-image-slice: 1;
  border-width: 5px;
  border-image-source: linear-gradient(to left, #5F8BEF, #42D392);
}

.selected{
  border-bottom: 2px solid;
  border-image-slice: 1;
  border-width: 5px;
  border-image-source: linear-gradient(to left, #5F8BEF, #42D392);
}

.selected:hover{
  border: none;
}


</style>