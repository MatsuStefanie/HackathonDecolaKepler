<template>
    <div class="teste-for">
        <h2> Teste for</h2>
        <ul>
            <li v-for="space of espaco" :key="space.id">
                <img :src="space.url" :alt="space.nome"/>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'TesteFor',
    data(){
        return{
             espaco:[
                {
                    id: 1
                    ,nome: 'estrelaNegra'
                    , url: 'https://www.revistaplaneta.com.br/wp-content/uploads/sites/3/2020/06/buraconegro-1.jpg'
                },
                {
                    id: 2
                    , nome: 'planeta'
                    , url: 'https://ibcdn.canaltech.com.br/0gTMi01SX4nXyUEWtcz_dUtiK1o=/512x288/smart/i222705.jpeg'
                },
                {
                    id: 3
                    , nome: 'planeta'
                    , url: 'https://www.revistaplaneta.com.br/wp-content/uploads/sites/3/2020/06/buraconegro-1.jpg'
                }
             ]
        }
    }
}
</script>

<style scoped>
    img{
        width: 800px;
        height: 400px;
    }
</style>