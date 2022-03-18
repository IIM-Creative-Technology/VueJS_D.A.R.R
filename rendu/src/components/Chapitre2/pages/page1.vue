<template>
<div class="page1">
    <h2>Dans ce cours nous allons apprendre les bases des evenements de Vue.js</h2>
    <p>On veut que si on click sur le bouton A un paragraphe avec la lettre A apparaisse</p>
    <button v-on:click="a = true">A</button>
    <p v-if="a == true">A</p>
    <p>On veut que si on click sur le bouton B un paragraphe avec la lettre B apparaisse</p>
    <button v-on:click="b = true">B</button>
    <p v-if="b == true">B</p>
    <p>On veut que si on click sur le bouton Other un paragraphe avec le mot other apparaisse</p>
    <button v-on:click="other = true">other</button>
    <p v-if="other == true">other</p>
</div>  
</template>

<script>
export default {
    data(){
        return {
            a: false,
            b: false,
            other: false
        }
    }
}
</script>

<style scoped>
h2 {
    text-align: center;
}
</style>