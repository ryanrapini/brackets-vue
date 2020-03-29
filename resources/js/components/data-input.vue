<template>
    <div class="row justify-content-center">
        <div class="col-sm">
            <div class="form-group">
                <label for="data-box">Data (json)</label>
                <textarea class="form-control" id="data-box" rows="3" v-model="input" @input="applyData"></textarea>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data: function() {
            return {
                input: ''
            }
        },
        methods: {
            applyData: function() {
                this.$store.commit('apply', this.input);
            }
        }
    }
</script>
