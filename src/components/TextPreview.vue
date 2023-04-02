<template>
    <b-card no-body class="print-preview-component">
        <b-form-textarea id="textarea"
            :value="text"
            rows="4"
            readonly>
        </b-form-textarea>
    </b-card>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
    props: {
        text: {
            type: String,
            default: ''
        }
    },
    data() {
        return {
            textResult: ''
        }
    },
    watch: {
        text (value:string) {
            this.textResult = value
        }
    },
})
</script>

<style lang="scss" scoped>
textarea {
    font-family: 'Courier New', Courier, monospace;
}
</style>
