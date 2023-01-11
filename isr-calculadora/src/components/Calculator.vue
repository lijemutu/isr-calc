<script>
export default {
    data() {
        return {
            periodicidad: '',
            ingreso:'',
        }
    },
    methods:{
        total(){
            return '$'+this.ingreso
        },
        impuestos(){
            return '$' + this.ingreso
        }
    }
}
</script>

<template>
    <div class="p-8">
        <label class="block text-white" for="periodicidadIngreso">¿Cada cuándo recibes tu ingreso?:</label>
        <br>
        <div class="columns-3 gap-8">
            <select class="block bg-neutral-800 text-white" id="periodicidadIngreso" v-model="periodicidad">
                <option value="" selected disabled required>Periodo</option>
                <option value="semanal">Semanal</option>
                <option value="quincenal">Quincenal</option>
                <option value="mensual">Mensual</option>
            </select>
            <input class="block bg-neutral-800 text-white" type="number" v-model.number="ingreso" placeholder="Ingreso $">
        </div>


        <div v-if="ingreso !=='' && periodicidad !=='' " class="text-white pt-5">
            <h2>Recibes despues de impuestos:</h2>
            <br>
            <h2>{{ total() }}</h2>
            <br>
            <h3>Pagas de impuestos:</h3>
            <br>
            <h3>{{ impuestos() }}</h3>
        </div>
    </div>

</template>

<style>

</style>