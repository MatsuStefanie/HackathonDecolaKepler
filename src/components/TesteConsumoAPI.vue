<template>
    <div class="teste-consumo-api">
        <h2> Sites favoritos</h2>
        <div v-for="site of sitesFavoritos" :key="site.id">
            <button>
                <a  :href="site.link"> 
                    {{site.nome}} 
                </a>
            </button>
        </div> 
    </div>
</template>

<script>
export default {
    nome: 'TesteConsumoAPI',
    data(){
        return{
            sitesFavoritos:[]
        }
    },
    created(){
        fetch('https://hackthon-decola.firebaseio.com/sites-favoritos.json')
            .then(result => result.json())
            .then(json => {
                this.sitesFavoritos = json;
            })
    }
}
</script>

<style>

</style>