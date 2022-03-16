<script setup>
import HeaderVue from './components/nav-1.vue'
import Chapter1Vue from './components/Chapter1.vue'
import Chapter2Vue from './components/Chapter2.vue'
import Chapter3Vue from './components/Chapter3.vue'
import Chapter4Vue from './components/Chapter4.vue'
import Chapter5Vue from './components/Chapter5.vue'

</script>

<template>
<HeaderVue></HeaderVue> 
<section class="main">
  <h1>Chapter{{count}}</h1>
  <div class="content">
  <Chapter1Vue></Chapter1Vue> 
  <Chapter2Vue></Chapter2Vue> 
  <Chapter3Vue></Chapter3Vue> 
  <Chapter4Vue></Chapter4Vue> 
  <Chapter5Vue></Chapter5Vue> 
  </div>
  <div class="end">
      <p class="counter">{{count}}/5</p>
      <button class="btn-next"><img src="./assets/next.png"></button>
  </div>
</section>

</template>

<script>

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
  margin-top: -50px;
  background-color: #E4E4E4;
  display: flex;
  justify-self: center;
  align-items: center;
  flex-direction: column;
  border-radius: 65px;
}

.content{
  display: flex;
  justify-self: center;
  align-content: center;
  width: 100%;
  height: 80%;
  background-color: red;
}


.end{
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-content: center;
  align-self: center;
  flex-direction: row;
  margin: 10px;
}

.btn-next {
  width: 72px;
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

.counter{
  font-style: normal;
  font-weight: 900;
  font-size: 48px;
  text-align: center;
  color: #000000;
  margin-left: 20px;
}
</style>