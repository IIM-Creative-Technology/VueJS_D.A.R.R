<template>
    <div id="app">
        <section id="chapter">
            <nav>
                <h2>Vue.js</h2>
                <h1>{{posts[count].title}}</h1>
            </nav>
            <div class="content_chapter">
                <ul class="list_chapter">
                    <button @click="chap1()">Chapter1</button>
                    <button @click="chap2()">Chapter2</button>
                    <button @click="chap3()">Chapter3</button>
                </ul>
                <ul class="tuto_chapter">
                    <p>{{posts[count].text1}}</p>
                    <p>{{posts[count].text1}}</p>
                    <p>{{posts[count].text1}}</p>
                    <p>{{posts[count].text2}}</p>
                    <p>{{posts[count].text1}}</p>
                    <p>{{posts[count].text1}}</p>
                    <p>{{posts[count].text1}}</p>
                </ul>
                <ul class="chapter_slide">
                    <div class="slide"></div>
                </ul>
            </div>
            
        </section>
    </div>
    
</template>
<style>
img{
    width: 100px;
    height: 100px;
}
</style>
<script>
export default {
    data() {
    return {
        count : 0,
        posts:[
            {   
                id:1, 
                title:"Chapter1", 
                text1:"Chap1 ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum",
                img1:""
            }, 
            {
                id:2, 
                title:"Chapter2",
                text1:"Chap2 ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum",
                text2:"Chap2 ipsum dolor sit amet, . Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum",
            }, 
            {
                id:3, 
                title:"Chapter3",
                text1:"Chap3 ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum",
            }]
    }
  },
  methods:{
    chap1: function () {
        this.count = 0;
    },
    chap2: function () {
        this.count = 1;
    },
    chap3: function () {
        this.count = 2;
    }
  
}
}

</script>   