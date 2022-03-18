<template>
    <div class="page3">
        <div class="blq3"></div>
        <p>Si vous regardez le composant App.vue vous trouvez la même organisation en 3 parties :</p>

        <p>c'est le composant de base de Vue js</p>

        <p>Maintenant parlons de cette balise</p>

        <p class="long"> &lt;HelloWorld msg="Welcome to Your Vue.js App""/&gt;</p>

        <p>Vous ne connaissez certainement pas la balise HelloWorld, c’est la façon qu’à Vue.js pour intégrer un composant dans un template tout simplement en créant une balise avec le nom du composant. Donc ici dans le template on dit :</p>
        <p>insérer le composant HelloWorld</p>
        <p>lui transmettre une variable avec l’attribut msg</p>

        <p>ainsi à la manière de cet exemple c'est ici que l'on déclare ses composants</p>


        <p>Utiliser une balise avec le nom du composant ne suffit pas, il faut aussi charger le composant dans la partie &lt;script&gt;:</p>


        <div class="code-zone long">
        &lt;script&gt;
        <br>import HelloWorld from './components/HelloWorld.vue'
        <br>
        export default {
            <br>'App',
                <br>description: 'Hello'components: {
                    <br>HelloWorld
                <br>}
        <br>}
        <br>&lt;/script&gt;
        </div>

    </div>
</template>

<style>

.blq3{
    width: 100px;
    height: 100px;
    margin-top: 400px;
}
.long{
    width: 90%;
}
</style>