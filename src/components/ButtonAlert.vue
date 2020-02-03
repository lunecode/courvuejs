<template>
<div>
  <b-button size="sm" @click="toggle">
    {{ show ? 'Hide' : 'Show' }} Alert
  </b-button>
  <b-alert
    v-model="show"
    class="mt-3"
    dismissible
    @dismissed="dismissed"
  >
    Hello {{ name }}!
  </b-alert>
</div>
</template>


<script>
export default {
    
    data() {
        return {
            name: 'le monde',
            show: true
        }
    },

    watch() {
        return {
            show(newVal) {
                'Alert is now ' + (newVal ? 'visible' : 'hidden')
            }
        }
    },

    methods() {
        return {
            toggle() {
                'Toggle button clicked'
                this.show = !this.show
            },

            dismissed() {
                'Alert dismissed'
            }
        }
    }
}
</script>