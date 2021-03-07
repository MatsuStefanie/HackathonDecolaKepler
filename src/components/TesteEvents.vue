<template>
    <div class="teste-events">
        <h2> Teste events </h2>
            <p v-for="frase of frases" :key="frase.id" @click="upcase(frase.id)">{{ frase.texto }}</p>
    </div>
</template>

<script>
export default {
    nome: 'TesteEvents',
    data(){
        return{
            frases: [
                {
                    id: 0,
                    texto:"A via lactia não é feita de leite, mas a lua parece um queijo"
                },
                {
                    id: 1,
                    texto: "Queijo, o rato roeu a roupa do rei de Roma rolando reto"
                },
                {
                    id: 2,
                    texto:"A via lactia não é feita de leite, mas a lua parece um queijo"
                },
                {
                    id: 3,
                    texto: "Queijo, o rato roeu a roupa do rei de Roma rolando reto"
                }
            ]
        }
    },
    methods:{
        upcase(index){
            this.frases[index].texto =  this.frases[index].texto.toUpperCase();
        }
    }
}
</script>

<style>

</style>