<template>
    <div class="um-contador">
        <h2> Um contador
        </h2>
        <p>
            <strong>
                Contador :
            </strong>
            {{ contador }}
        </p>
        <button @click="subtraiUm">
            -
        </button>
        <button @click="somaUm">
            +
        </button>
    </div>
</template>

<script>
export default {
    name: 'UmContador',
    data(){
        return{
            contador: '0'
        }
    },
    methods:{
        somaUm(){
            this.contador++;
        },
        subtraiUm(){
            this.contador--;
        }
    }
}
</script>

<style>

</style>