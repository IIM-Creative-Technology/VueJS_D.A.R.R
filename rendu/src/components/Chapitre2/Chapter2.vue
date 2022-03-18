<script setup>
    import page0Vue from "./pages/page0.vue"
    import page1Vue from "./pages/page1.vue"
    import page2Vue from "./pages/page2.vue"
    import page3Vue from "./pages/page3.vue"
    import page4Vue from "./pages/page4.vue"
</script>

<template>
    <section class="chapter2">
        <page0Vue v-if="count == 0"></page0Vue>
        <page1Vue v-if="count == 1"></page1Vue>
        <page2Vue v-if="count == 2"></page2Vue>
        <page3Vue v-if="count == 3"></page3Vue>
        <page4Vue v-if="count == 4"></page4Vue>
    </section>
    <div class="end">
        <button class="btn-before" v-on:click="count -= 1" @click="beforeChapter" v-if="count > 0"><img src="../../assets/next.png"></button>
        <p class="counter">{{count}}/4</p>
        <button class="btn-next" v-on:click="count += 1" @click="nextChapter" v-if="count < 4"><img src="../../assets/next.png"></button>
  </div>
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

      if(this.count > 5){
        this.count = 0
      }
    },
    beforeChapter(){
      
      console.log(this.count)

      if(this.count <= 0){
        this.count = 0
      }
    }
  },
  
}
</script>


<style>
.page0{
    width: 100%;
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.page2{
    overflow-y:scroll;
}
</style>