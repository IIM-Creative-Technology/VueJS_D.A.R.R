<template>
    <nav>
        <a href="" class="logo"><img src="../assets/Vuejs.png" alt=""></a>
        <div class="dark" v-if="mode == 1">
            <input @input="dark" class="dm" type="checkbox" id="dm">
            <label for="dm"></label>
        </div>
        <div class="light" v-if="mode == 0">
            <input @input="light" class="dm" type="checkbox" id="dm">
            <label for="dm"></label>
        </div>
    </nav>
</template>

<style scoped>
.logo > img{
    margin: 50px;
}

nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-right: 40px;
}

.dark{
    width: 60px;
    height: 25px;
    display: flex;
    justify-content: center;
    align-items: center;
    
}

.divDm > .dm:checked + label{
    

}

.dark > .dm + label {
    width: 100%;
    height: 100%;
    background-color: black;
    border-radius: 25px;
    display: flex;
    justify-content:start;
    align-items: center;
    padding: 2px;
}

.dark > .dm + label::before {
    content: " ";
    width: 20px;
    height: 20px;
    background-color: red;
    border-radius: 25px;
    cursor: pointer;
}

.dm{
    opacity: 0;
    width: 0;
}
</style>

<script>
export default {
    data(){
        return {
            mode: 0
        }
    },
    methods:{
        dark(){
            mode++
            document.body.style.backgroundColor = "black"
            document.h4.style.Color = "white"
        },
        light(){
            mode--
            document.body.style.backgroundColor = "white"
            document.h4.style.Color = "black"
        }
    }
}
</script>