<script setup>
import page5 from './page5.vue'
import page1Vue from './page1.vue'
import page2Vue from './page2.vue'
import page3Vue from './page3.vue'
import page4Vue from './page4.vue'
import page5Vue from './page5.vue'
</script>

<template>
    <section class="chapter1">
        <page1Vue v-if="count == 1"></page1Vue>
        <page2Vue v-if="count == 2"></page2Vue>
        <page3Vue v-if="count == 3"></page3Vue>
        <page4Vue v-if="count == 4"></page4Vue>
        <page5Vue v-if="count == 5"></page5Vue>
    </section>
    <div class="end">
        <button class="btn-before" v-on:click="count -= 1" @click="beforeChapter"><img src="../assets/next.png"></button>
        <p class="counter">{{count}}/5</p>
        <button class="btn-next" v-on:click="count += 1" @click="nextChapter"><img src="../assets/next.png"></button>
  </div>
</template>

<script>
export default {
  components: { page5 },
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
.chapter1{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-content: center;
    flex-direction: column;
}


.page1{
    width: 100%;
    height: 250%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    overflow-y: scroll;
}

.start{
    width: 80%;
    text-align: center;
}

p{
    width: 80%;
    text-align: start;
}

.code-zone{
    width: 50%;
    background-color: black;
    color: white;
    display: flex;
    justify-content: start;
    align-items: start;
    padding: 10px;
    border-radius: 10px;
    margin: 20px;

}
.page2{
    width: 100%;
    height: 100%;
    overflow-y: scroll;
}
.page3{
    width: 100%;
    height: 100%;
    overflow-y: scroll;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.page4{
    width: 100%;
    height: 100%;
    overflow-y: scroll;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.page5{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    overflow-y: scroll;
}

.q1{
    display: flex;
    justify-content: center;
    align-items: start;
    flex-direction: column;
    text-align: left;
}

.q1 > div{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
}



#yesQ1:checked + .trueQ1{
    color: green;
}


#yesQ1:checked{
    width: 0;
    opacity: 0;
}

#noQ1:checked + .falseQ1{
    color: red;
}

#noQ1:checked{
    width: 0;
    opacity: 0;
}

.q2{
    display: flex;
    justify-content: center;
    align-items: start;
    flex-direction: column;
    text-align: center;
}

.q2 > div{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
}

#yesQ2:checked + .trueQ2{
    color: green;
}

#yesQ2:checked{
    width: 0;
    opacity: 0;
}

#noQ2:checked + .falseQ2{
    color: red;
}

#noQ2:checked{
    width: 0;
    opacity: 0;
}

.q3{
    display: flex;
    justify-content: center;
    align-items: start;
    flex-direction: column;
    text-align: center;
}

.q3 > div{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
}

#yesQ3:checked + .trueQ3{
    color: green;
}

#yesQ3:checked{
    width: 0;
    opacity: 0;
}

#noQ3:checked + .falseQ3{
    color: red;
}

#noQ3:checked{
    width: 0;
    opacity: 0;
}





.end{
  width: 90%;
  display: flex;
  justify-content: space-between;
  align-content: center;
  align-self: center;
  flex-direction: row;
  margin: 10px;
  

}
</style>

