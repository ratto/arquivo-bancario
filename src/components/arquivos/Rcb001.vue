<template>
    <div class="rcb001-file">
        <p>{{ text }}</p>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
    name: 'Rcb001',
    props: {
        fnChangeText: {
            type: Function,
            required: true
        }
    },
    data () {
        return {
            text: ''
        }
    },
    mounted () {
        this.text = 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nulla, fuga est? Eveniet itaque eum illum nostrum unde fugiat non quas officia vero deserunt vitae expedita minus, exercitationem provident praesentium nemo?'
    },
    watch: {
        text (value) {
            this.fnChangeText(value)
        }
    }
})
</script>
