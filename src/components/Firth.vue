<template>
    <div class="ny">
        <!-- <p> {{ fullText }} </p>        -->
        <div id="demo">{{ fullName }}</div>
    </div>
</template>


 <script>
    // var vm = new Vue({
    // el: '#demo',
    // data: {
    //     firstName: 'Foo',
    //     lastName: 'Bar',
    //     fullName: 'Foo Bar'
    // },
    // watch: {
    //     firstName: function (val) {
    //     this.fullName = val + ' ' + this.lastName
    //     },
    //     lastName: function (val) {
    //     this.fullName = this.firstName + ' ' + val
    //     }
    // }
    // })


export default {
 
    data() {
        return {
        firstName: 'Foo',
        lastName: 'Bar'
        }
    },
    computed: {
        fullName: function () {
            return this.firstName + ' ' + this.lastName
            }
    }
}

// export default {
//     data() {
//         return {
//             hello : "Hello",
//             word : "Word", 
//          }
//     },
//     computed: {
//         fullText: {
//             // GETTER
//             get: function () {
//                 return this.hello + ' ' + this.word
//             },
//             // SETTER
//             set: function (fullText) {
//                 const newHelloWord= fullText.split(' ') 
//                 this.hello= newHelloWord[0]     
//                 this.word= newHelloWord[newHelloWord.length - 1]
//             }

//         } 
//     },
// }
</script>



<style>
.ny {
    border:  2px yellow solid;
}
</style>
