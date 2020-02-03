<template>
    <div class="na">
      
        <div>
            {{ fullText }} 
            <p> {{ longText(word, chemin) }}  </p>
        </div>
   </div>

</template>

<script>

export default {
    data() {
         return {
            hello : "Hello",
            word : "Word",
            chemin: "naaaaa"
         }
    },

    computed: {
        // methode 1
        fullText() {
            return this.hello + (' ') + this.word;
        },
        // methode 2
        longText() {
            return function fulltext(mot, na) {
                return this.hello + ' ' + mot + ' ' + na 
            }
        },     
    }
}

</script>


<style>
.na {
    border:  2px red solid;
}
</style>
