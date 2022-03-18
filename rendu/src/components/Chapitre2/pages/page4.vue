<template>
 <div class="page4" v-if="count = 3">
            <h2>Quizz</h2>
            <h2>Question 1 :</h2>
                <h4>Ya t-il une diff entre @click :onclick ?</h4>
                <div class="q1">
                    <div>
                        <input type="checkbox" id="noQ1"> 
                        <label class="falseQ1"> Oui</label>
                    </div>
                    <div>
                        <input type="checkbox" id="yesQ1"> 
                        <label class="trueQ1" for="yesQ1">non</label>
                    </div>
                </div>
            <h2>Question 2 – Création :</h2>
                <h4>{ {count} } ou (count) ?</h4>
                <div class="q2">
                    <div>
                        <input type="checkbox" id="yesQ2"> 
                        <label class="trueQ2">{ {count} }</label>
                    </div>
                    <div>
                        <input type="checkbox" id="noQ2" > 
                        <label class="falseQ2">(count)</label>
                    </div>
                </div>
            <h2>Question 3 :</h2>
                <h4>this.letter = "A" ou this.letter = A</h4>
                <div class="q3">
                    <div>
                        <input type="checkbox" id="noQ3" > 
                        <label class="trueQ3" >this.letter = "A"</label>
                    </div>
                    <div>
                        <input type="checkbox" id="yesQ3"> 
                        <label class="trueQ3"> this.letter = A</label>
                    </div>
                </div>
        </div>
</template>