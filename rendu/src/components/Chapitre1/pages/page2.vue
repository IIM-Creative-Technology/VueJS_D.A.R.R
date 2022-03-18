<template>
<div class="page1">
    <div class="blq2"></div>
    <p>Maintenant voyons ensemble comment marche l'infrastructure de base que vous avez sous les yeux</p>

<p>node_modules : toutes les dépendances nécessaires au projet chargées par npm à partir de la configuration de package.json</p>

<div class="code-zone">public/index.html</div><p> ^ Le fichier HTML d’entrée du projet</p>

<div class="code-zone">src/main.js</div> <p> ^ Le fichier Javascript de configuration du projet</p>

<div class="code-zone">src/App.vue</div>
 <p>^ Le composant de base de l’application. Les composants sont les pièces de construction de Vue.js et comportent du HTML, du CSS et du Javascript</p>


<div class="code-zone">src/components/HelloWorld.vue</div>
<p>encore un composant, c’est lui qui affiche la page de présentation vue qui se présente sur l'écran</p>


<div class="code-zone">src/assets</div>
<p>un dossier pour les éléments statiques du projet comme les images</p>

<p>
Parlons maintenant plus en profondeurs de quelques fichiers:


Au sein du composant Hello world vous trouverez trois grandes parties

Le &lt;template&gt; contient tout le HTML du composant, donc la structure du composant.

la partie &lt;style&gt; est l'endroit contenant le CSS du composant, donc la gestion de l’apparence. Notez au passage le commentaire qui indique d’ajouter scoped pour limiter le style au composant.</p>

<p>enfin la partie &lt;script&gt; c’est le moteur Javascript du composant, on reviendra sur le code plus tard.</p>
</div>
</template>

<style>
.blq2{
    width: 100px;
    height: 100px;
    margin-top: 700px;
}
</style>