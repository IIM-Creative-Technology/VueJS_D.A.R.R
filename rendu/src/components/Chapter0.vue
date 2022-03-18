<script setup>
import { count } from "../App.vue"

</script>

<template>
    <section class="chapter1">
        <div class="page1" v-if="count == 1">
            
        </div>
        <div class="page2" v-if="count == 2">
            
        </div>
        <div class="page3" v-if="count == 3">
            
        </div>
    </section>
    
</template>

<script>
export default {
    data() {
        return {
            count
        }
    },
    methods: {
        test(){
            console.log(this.count)
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


.end{
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-content: center;
  align-self: center;
  flex-direction: row;
  margin: 10px;
}
</style>

