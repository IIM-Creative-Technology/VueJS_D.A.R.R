<template>
    <div class="page3">
        <p>Et enfin nos data ainsi que les functions qui mettrons à jours ces mêmes datas</p>
        <div class="code-zone">
        <br>export default {
        <br>data() {
            <br>return {
                <br>letter : ""
            <br>}
        <br>},
        <br>methods:{
            <br>a: function () {
                <br>this.letter = "A"
            <br>},
            <br>b: function () {
                <br>this.letter = "B"
            <br>},
            <br>other: function () {
                <br>this.letter = "other"
            <br>}
        <br>},
        <br>
        <br>}
        </div>
    </div>

    
</template>

<style scoped>
    .code-zone{
        width: 80%;
    }
    </style>