<template>
    <div class="sites-favoritos">
        <h2>Séries Favoritas</h2>
        <ul>
            <li
             v-for="site of sitesFavoritos"
             :key="site.id"
             >
                <a :href="site.link">{{ site.nome }}</a>
            </li>
        </ul>

    </div>
</template>

<script>
export default {
    name: 'SitesFavoritos',
    data(){
        return{
            sitesFavoritos: []
        }
    },
    created() {
        fetch('https://hackthon-decola.firebaseio.com/sites-favoritos.json')
        .then(response => response.json())
        .then(json =>{
            this.sitesFavoritos = json
        })
    }
}
</script>

<style lang="less" scoped>

</style>