<script>
export default {
    data() {
        return {
            periodicidad: '',
            ingreso: '',
        }
    },
    methods: {
        total22() {
            let ingresoF = parseFloat(this.ingreso)
            return (ingresoF - this.impuestos22()).toFixed(2)
        },
        impuestos22() {
            let ingresoF = parseFloat(this.ingreso)
            let impuestos = (ingresoF - this.limiteInferiorMensual22(ingresoF)) * this.porcentajeExcMensual22(ingresoF) + this.cuotaMensual22(ingresoF)
            return impuestos.toFixed(2)
        },
        limiteInferiorMensual22(ingreso) {
            let ingresoF = parseFloat(ingreso);
            if (ingresoF >= 0.01 && ingresoF < 644.58) {
                return 0.01
            }
            if (ingresoF >= 644.59 && ingresoF < 5470.92) {
                return 644.59
            }
            if (ingresoF >= 5470.93 && ingresoF < 9614.66) {
                return 5470.93
            }
            if (ingresoF >= 9614.67 && ingresoF < 11176.62) {
                return 9614.67
            }
            if (ingresoF >= 11176.63 && ingresoF < 13381.47) {
                return 11176.63
            }
            if (ingresoF >= 13381.48 && ingresoF < 26988.50) {
                return 13381.48
            }
            if (ingresoF >= 26988.51 && ingresoF < 42537.58) {
                return 26988.51
            }
            if (ingresoF >= 42537.59 && ingresoF < 81211.25) {
                return 42537.59
            }
            if (ingresoF >= 81211.26 && ingresoF < 108281.67) {
                return 81211.26
            }
            if (ingresoF >= 108281.68 && ingresoF < 324845.01) {
                return 108281.68
            }
            if (ingresoF >= 324845.02) {
                return 324845.02
            }
        },

        cuotaMensual22(ingreso) {
            let ingresoF = parseFloat(ingreso);
            if (ingresoF >= 0.01 && ingresoF < 644.58) {
                return 0
            }
            if (ingresoF >= 644.59 && ingresoF < 5470.92) {
                return 12.38
            }
            if (ingresoF >= 5470.93 && ingresoF < 9614.66) {
                return 321.26
            }
            if (ingresoF >= 9614.67 && ingresoF < 11176.62) {
                return 772.1
            }
            if (ingresoF >= 11176.63 && ingresoF < 13381.47) {
                return 1022.1
            }
            if (ingresoF >= 13381.48 && ingresoF < 26988.50) {
                return 1417.12
            }
            if (ingresoF >= 26988.51 && ingresoF < 42537.58) {
                return 4323.58
            }
            if (ingresoF >= 42537.59 && ingresoF < 81211.25) {
                return 7980.73
            }
            if (ingresoF >= 81211.26 && ingresoF < 108281.67) {
                return 19582.83
            }
            if (ingresoF >= 108281.68 && ingresoF < 324845.01) {
                return 28245.36
            }
            if (ingresoF >= 324845.02) {
                return 101876.90
            }
        },

        porcentajeExcMensual22(ingreso) {
            let ingresoF = parseFloat(ingreso);
            if (ingresoF >= 0.01 && ingresoF < 644.58) {
                return 1.92 * 0.01
            }
            if (ingresoF >= 644.59 && ingresoF < 5470.92) {
                return 6.4 * 0.01
            }
            if (ingresoF >= 5470.93 && ingresoF < 9614.66) {
                return 10.88 * 0.01
            }
            if (ingresoF >= 9614.67 && ingresoF < 11176.62) {
                return 16 * 0.01
            }
            if (ingresoF >= 11176.63 && ingresoF < 13381.47) {
                return 17.92 * 0.01
            }
            if (ingresoF >= 13381.48 && ingresoF < 26988.50) {
                return 21.36 * 0.01
            }
            if (ingresoF >= 26988.51 && ingresoF < 42537.58) {
                return 23.52 * 0.01
            }
            if (ingresoF >= 42537.59 && ingresoF < 81211.25) {
                return 30 * 0.01
            }
            if (ingresoF >= 81211.26 && ingresoF < 108281.67) {
                return 32 * 0.01
            }
            if (ingresoF >= 108281.68 && ingresoF < 324845.01) {
                return 34 * 0.01
            }
            if (ingresoF >= 324845.02) {
                return 35 * 0.01
            }
        },

        total23() {
            let ingresoF = parseFloat(this.ingreso)
            return (ingresoF - this.impuestos23()).toFixed(2)
        },
        impuestos23() {
            let ingresoF = parseFloat(this.ingreso)
            let impuestos = (ingresoF - this.limiteInferiorMensual23(ingresoF)) * this.porcentajeExcMensual23(ingresoF) + this.cuotaMensual23(ingresoF)
            return impuestos.toFixed(2)
        },
        limiteInferiorMensual23(ingreso) {
            let ingresoF = parseFloat(ingreso);
            if (ingresoF >= 0.01 && ingresoF < 746.04) {
                return 0.01
            }
            if (ingresoF >= 746.05 && ingresoF < 6332.05) {
                return 746.05
            }
            if (ingresoF >= 6332.06 && ingresoF < 11128.01) {
                return 6332.06
            }
            if (ingresoF >= 11128.02 && ingresoF < 12935.82) {
                return 11128.02
            }
            if (ingresoF >= 12935.83 && ingresoF < 15487.71) {
                return 12935.83
            }
            if (ingresoF >= 15487.72 && ingresoF < 31236.49) {
                return 15487.72
            }
            if (ingresoF >= 31236.50 && ingresoF < 49233) {
                return 31236.50
            }
            if (ingresoF >= 49233.01 && ingresoF < 93993.90) {
                return 49233.01
            }
            if (ingresoF >= 93993.91 && ingresoF < 125325.20) {
                return 93993.91
            }
            if (ingresoF >= 125325.21 && ingresoF < 375975.61) {
                return 125325.21
            }
            if (ingresoF >= 375975.61) {
                return 375975.61
            }
        },

        cuotaMensual23(ingreso) {
            let ingresoF = parseFloat(ingreso);
            if (ingresoF >= 0.01 && ingresoF < 746.04) {
                return 0.0
            }
            if (ingresoF >= 746.05 && ingresoF < 6332.05) {
                return 14.32
            }
            if (ingresoF >= 6332.06 && ingresoF < 11128.01) {
                return 371.83
            }
            if (ingresoF >= 11128.02 && ingresoF < 12935.82) {
                return 893.63
            }
            if (ingresoF >= 12935.83 && ingresoF < 15487.71) {
                return 1182.88
            }
            if (ingresoF >= 15487.72 && ingresoF < 31236.49) {
                return 1640.18
            }
            if (ingresoF >= 31236.50 && ingresoF < 49233) {
                return 5004.12
            }
            if (ingresoF >= 49233.01 && ingresoF < 93993.90) {
                return 9236.89
            }
            if (ingresoF >= 93993.91 && ingresoF < 125325.20) {
                return 22665.17
            }
            if (ingresoF >= 125325.21 && ingresoF < 375975.61) {
                return 32691.18
            }
            if (ingresoF >= 375975.61) {
                return 117912.32
            }
        },

        porcentajeExcMensual23(ingreso) {
            let ingresoF = parseFloat(ingreso);
            if (ingresoF >= 0.01 && ingresoF < 746.04) {
                return 1.92 * 0.01
            }
            if (ingresoF >= 746.05 && ingresoF < 6332.05) {
                return 6.4 * 0.01
            }
            if (ingresoF >= 6332.06 && ingresoF < 11128.01) {
                return 10.88 * 0.01
            }
            if (ingresoF >= 11128.02 && ingresoF < 12935.82) {
                return 16 * 0.01
            }
            if (ingresoF >= 12935.83 && ingresoF < 15487.71) {
                return 17.92 * 0.01
            }
            if (ingresoF >= 15487.72 && ingresoF < 31236.49) {
                return 21.36 * 0.01
            }
            if (ingresoF >= 31236.50 && ingresoF < 49233) {
                return 23.52 * 0.01
            }
            if (ingresoF >= 49233.01 && ingresoF < 93993.90) {
                return 30 * 0.01
            }
            if (ingresoF >= 93993.91 && ingresoF < 125325.20) {
                return 32 * 0.01
            }
            if (ingresoF >= 125325.21 && ingresoF < 375975.61) {
                return 34 * 0.01
            }
            if (ingresoF >= 375975.61) {
                return 35 * 0.01
            }
        }
    }
}
</script>

<template>
    <div class="p-8">
        <label class="block text-neutral-100" for="periodicidadIngreso">¿Cada cuándo recibes tu ingreso?:</label>
        <br>
        <div class="columns-3 gap-8">
            <select class="block bg-neutral-800 text-neutral-100" id="periodicidadIngreso" v-model="periodicidad">
                <option value="" selected disabled required>Periodo</option>
                <option value="semanal">Semanal</option>
                <option value="quincenal">Quincenal</option>
                <option value="mensual">Mensual</option>
            </select>
            <input class="block bg-neutral-800 text-neutral-100" type="number" v-model.number="ingreso"
                placeholder="Ingreso $">
        </div>


        <div v-if="ingreso !== '' && periodicidad !== ''" class="text-neutral-100 pt-5">
            <h2>Recibes despues de impuestos en 2022:</h2>
            <br>
            <h2>${{ total22() }}</h2>
            <br>
            <h3>Pagabas de impuestos en 2022:</h3>
            <br>
            <h3>${{ impuestos22() }}</h3>
            <br>

            <h2>Recibes despues de impuestos en 2022:</h2>
            <br>
            <h2>${{ total23() }}</h2>
            <br>
            <h3>Pagabas de impuestos en 2022:</h3>
            <br>
            <h3>${{ impuestos23() }}</h3>

            <h2>Despues de la reforma ahora ganas {{ total23() > total22() ? "más" : "menos"}}: <span :class="total23() > total22() ? 'text-green-500' : 'text-red-500'">${{ (total23() - total22()).toFixed(2) }}</span></h2>
        </div>
    </div>

</template>

<style>

</style>