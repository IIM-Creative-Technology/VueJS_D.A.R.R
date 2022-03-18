<template>
    <div class="page3">
    <p>Ce code simple et rapide à écrire fonctionne de la manière suivante : 
Nous importons tout d’abord nos différents fichiers vus et ensuite définissions nos routes avec une const. Cela permet au navigateur de savoir qu’elle template chargée en fonction de l’url
currentPath ensuite récupère les info après le / dans l’url
Un eventlistener sur cet hash change la valeur ainsi on garde toujours la valeur du hash actuelle.

Finalement nous déclarons un component (avec computed) appeler currentView
Se component return une route en fonction du hash dans l’url, comme la const routes est
Liée à des fichier vue, VueJS charge automatiquement ces fichiers, sur notre page et ainsi notre router fonctionne. </p>
    </div>
</template>