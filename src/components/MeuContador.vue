<template>
    <div class="meu-contador">
        <h2>Meu Contador</h2>
        <p><strong>Contador: </strong>{{  contador }}</p>
        <button @click="removeUm">-</button>
        <button @click="adicionaUm">+</button>
    </div>
    
</template>

<script>
export default {
    name:'MeuContador',
    data(){
        return{
            contador: 0
        }
    },
    methods: {
        removeUm() {
            this.contador--;
        },
        adicionaUm() {
            this.contador++;
        }
    }
}
</script>

<style scoped>

</style>>