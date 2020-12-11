<template>
    <div class="teste-if">
        <h2 v-if="podever">Agora você me Vue</h2>
        <h2 v-else>Agora você não me Vue</h2>

    </div>
</template>

<script>
export default {
    name: 'TesteIf',
    data(){
        return{
            podeVer: false
        }
    }
}
</script>

<style scoped>

</style>

