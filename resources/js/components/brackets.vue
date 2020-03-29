<template>
    <div class="row justify-content-center">
        <div class="col-sm" v-if="true">
            {{ $store.state.data }}
        </div>
        <div class="col-sm">
            <div class="form-group">
                <label for="data-box">Data (json)</label>
                <textarea class="form-control" id="data-box" rows="3"></textarea>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        mounted() {
            
        }
    }
</script>
