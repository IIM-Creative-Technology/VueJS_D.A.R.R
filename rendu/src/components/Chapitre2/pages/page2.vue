<template>
<div class="page2">
        <p>En premier temps on ajoutes nos paragraphe avec nos conditions, les V-if / v-else-if / v-els</p>
        <div class="code-zone">
        &lt;template&gt;
                <br>&lt;p v-if="type === 'A'"&gt; B &lt;/p&gt;
                <br>&lt;p v-else-if="type === 'B'"&gt; A&lt;/p&gt;
                <br>&lt;p v-else&gt; Other&lt;/p&gt;
        <br>&lt;/template&gt;
        </div>
    <p>En deuxième temps nos boutons</p>
        <div class="code-zone">
            <br>&lt;button @click="a()"&gt;a&lt;/button&gt;
            <br>&lt;button @click="b()""&gt;b&lt;/button&gt;
            <br>&lt;button @click="other()"&gt;other&lt;/button&gt;
        </div>
    <p>Et enfin nos data ainsi que les functions qui mettrons à jours ces mêmes datas</p>
    
</div>
</template>

<style scoped>
.code-zone{
    width: 80%;
}
</style>