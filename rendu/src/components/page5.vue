<template>
 <div class="page5" v-if="count = 3">
            <h2>Quizz</h2>
            <h2>Question 1 – Installation :</h2>
                <h4>Comment installer vue js cli ?</h4>
                <div class="q1">
                    <div>
                        <input type="checkbox" id="noQ1"> 
                        <label class="falseQ1"> vue@lastest</label>
                    </div>
                    <div>
                        <input type="checkbox" id="noQ1"> 
                        <label class="falseQ1">npm install vue cli</label>
                    </div>
                    <div>
                        <input type="checkbox" id="yesQ1"> 
                        <label class="trueQ1" for="yesQ1">npm install -g @vue/cli</label>
                    </div>
                </div>
            <h2>Question 2 – Création :</h2>
                <h4>Compléter cette phrase de création de fichier</h4>
                <h4>vue ___ 'filename' </h4>
                <div class="q2">
                    <div>
                        <input type="checkbox" id="yesQ2"> 
                        <label class="trueQ2">create</label>
                    </div>
                    <div>
                        <input type="checkbox" id="noQ2" > 
                        <label class="falseQ2">make</label>
                    </div>
                    <div>
                        <input type="checkbox" id="noQ2"> 
                        <label class="falseQ2">do</label>
                    </div>
                </div>
            <h2>Question 2 – Serveur :</h2>
                <h4>Comment lancer le serveur en local ?</h4>
                <div class="q3">
                    <div>
                        <input type="checkbox" id="noQ3" > 
                        <label class="falseQ3" >npm run dev</label>
                    </div>
                    <div>
                        <input type="checkbox" id="yesQ3"> 
                        <label class="trueQ3">npm run serve</label>
                    </div>
                    <div>
                        <input type="checkbox" id="noQ3" > 
                        <label class="falseQ3">npm start serve</label>
                    </div>
                </div>
        </div>
</template>