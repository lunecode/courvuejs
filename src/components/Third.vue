<template>
    <div class="no">
        <!-- propriété simple -->
        <div>
            <p> Message : {{ msg }} </p>
        </div>
        <!-- propriété calculée -->
        <div>
            <p> Message avec propriété calculée, seulement le 1er mot : {{ onlyFirstWord }} </p>
        </div>
      
   </div>

</template>

<script>

export default {
    data() {
         return {
            msg: 'lune rouge sombre',
         }
    },
    computed: {
        onlyFirstWord() {
            return this.msg.split(' ')[2].toUpperCase();
        },
    },
    created() {

    },
    mounted() {

    },
    methods: {

    }      
}

</script>

<style>
.no {
    border:  2px blue solid;
}

</style>
