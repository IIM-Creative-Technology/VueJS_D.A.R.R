<template>
    <section class="chapter2"></section>
    <div class="end">
        <button class="btn-before" v-on:click="count -= 1" @click="beforeChapter"><img src="../../assets/next.png"></button>
        <p class="counter">{{count}}/5</p>
        <button class="btn-next" v-on:click="count += 1" @click="nextChapter"><img src="../../assets/next.png"></button>
  </div>
</template>

<style>
.chapter2{
    background-color:lime;
}
</style>