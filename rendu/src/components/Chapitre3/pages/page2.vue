<template>
<div class="page3">
    <div class="code-zone">
                    <br>&lt;script setup&gt;
        <br>import { ref, computed } from 'vue'
        <br>import Home from './Home.vue'
        <br>import About from './About.vue'
        <br>import NotFound from './NotFound.vue'

        <br>const routes = {
        <br>'/': Home,
        <br>‘/about’: About,
        <br>}

        <br>const currentPath = ref(window.location.hash)

        <br>window.addEventListener('hashchange', () => {
        <br>currentPath.value = window.location.hash
        <br>})

        <br>const currentView = computed(() => {
        <br>  return routes[currentPath.value.slice(1) || '/'] || NotFound
        <br>})
        <br>&lt;/script&gt; 

        <br>&lt;template&gt;
        <br>  &lt;a href="#/"&gt;Home&lt;/a&gt; |
        <br>  &lt;a href="#/about"&gt;About&lt;/a&gt; 
        <br>  &lt;component :is="currentView" /&gt;
        <br>&lt;/template&gt; 
            </div>
</div>

</template>