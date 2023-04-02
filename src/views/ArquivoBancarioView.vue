<template>
    <div id="arquivo-bancario">
        <h1>Gerador de Arquivos Bancários</h1>
        <ArquivoBancario class="mb-3"
            @on-change="ChangeText($event)" />
        <TextPreview :text="text" />
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
import TextPreview from '@/components/TextPreview.vue'
import ArquivoBancario from '@/components/ArquivoBancario.vue'

export default Vue.extend({
    name: 'ArquivoBancarioView',
    components: {
        TextPreview,
        ArquivoBancario
    },
    data () {
        return {
            text: ''
        }
    },
    methods: {
        ChangeText (value:string) {
            this.text = value
        }
    }
})
</script>
