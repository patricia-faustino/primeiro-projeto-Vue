<template>
    <div class="teste-for">
        <ul>
            <li v-for="animal of animais" :key="animal.id">
                <p><strong>{{ animal.titulo }}</strong></p>
                <img :src="animal.url" :alt="animal.nome">
            </li>
        </ul>

    </div>
</template>

<script>
export default {
    name:'TesteFor',
    data(){
        return{
            animais:[
                {
                    id: 1,
                    nome: 'Gatinho',
                    url:'https://www.petz.com.br/blog/wp-content/uploads/2020/04/meu-primeiro-gato.jpg'
                },
                {
                    id:2,
                    nome: 'Cachorrinho',
                    url: 'https://image.cachorrogato.com.br/thumb/1200/630/1/imagens/original/imagem858.jpg'
                }
            ]
        }
    }
}
</script>

<style lang="less" scoped>

</style>