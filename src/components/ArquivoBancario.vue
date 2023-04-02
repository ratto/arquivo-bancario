<template>
    <div>
        <b-card no-body class="arquivo-bancario-componente">
            <b-card-body>
                <component :is="fileType" :fn-change-text="ChangeText" />
            </b-card-body>
        </b-card>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Rcb100 from './arquivos/Rcb001.vue'

export default Vue.extend({
    name: 'ArquivoBancario',
    components: {
        Rcb100
    },
    data () {
        return {
            fileType: Rcb100
        }
    },
    methods: {
        ChangeText (text:string) {
            this.$emit('on-change', text)
        }
    }
})
</script>
