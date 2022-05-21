<template>
    <div style="margin:3%;">
        <div style="display: flex; width: 100%; background-color: #005483; flex-wrap: wrap;">
            <div style="display: flex; flex-direction: column; justify-content: center; align-items: center; flex: 9;">
                <div style="width:60%" class="pt-5 pb-5">
                    <p style="font-weight: lighter;font-size:22px; font-weight: bold; color: #FFFFFF;">¿Cuándo debo
                        acudir al consultorio del <a style="color:#2397D7">DR. ALEJANDRO MESARINA</a>?</p>
                    <p style="font-weight: lighter;font-size:20px; color: #FFFFFF;">Puedes acudir a nosotros por
                        cualquier <a style="font-weight: bold ;color: #FFFFFF;">lesión o dolencia</a> que tengas <a
                            style="color: #FFFFFF;font-weight: bold;">con tu sistema musculo-esquelético y
                            articular</a>, de cualquier origen tanto <a
                            style="color: #FFFFFF;font-weight: bold;">traumatico</a> como <a
                            style="color: #FFFFFF;font-weight: bold; color: white;">degenerativo</a>, sea <a
                            style="font-weight: bold; color: white;">por ejemplo para el tratamiento</a> de una lesión
                        como es el caso de una <a style="font-weight: bold; color: white;">lesión de rodilla</a>, <a
                            style="font-weight: bold; color: white;">cadera</a>, <a
                            style="font-weight: bold; color:white;">tobillo</a>, <a
                            style="font-weight: bold; color:white;">muñeca</a> o una dolencia de la <a
                            style="font-weight: bold; color: white;">columna vertebral</a> o una condición desarrollada
                        a lo largo del tiempo como <a style="font-weight: bold; color: white;">osteoartrosis</a>.</p>
                    <p style="font-weight: lighter;font-size:20px; color: #FFFFFF;"><a
                            style="font-weight: bold; color: white;color: #FFFFFF;">Nuestro objetivo </a>es curar al
                        íntegro la lesión que te aqueja, y en lesiones crónicas e irreversibles reducir el dolor,
                        mejorar la movilidad y, sobre todo, la calidad de vida de nuestros pacientes.</p>
                </div>
            </div>
            <div interval="4000"
                style="display: flex; justify-content: center; align-items: center; height: 70vh; width: 500px;  flex: 4;">
                <v-carousel height="100%" id="base-doc-image" cycle hide-delimiters :show-arrows="false">
                    <v-carousel-item v-for="(img, i) in imgs" :key="i" v-bind:src="img">
                    </v-carousel-item>
                </v-carousel>
            </div>
        </div>
    </div>
</template>
<script>
import imgope1 from '../assets/IMG_1771.png'
import imgope2 from '../assets/ope.png'

export default {
    data: () => ({
        imgs: [
            imgope1,
            imgope2,
        ],
    }),
}
</script>
<style scoped>
.img-ope {

    background: url('../assets/ope.png') no-repeat;
    height: 60vh;
    background-size: cover;
    background-position: center;
    min-width: 300px;
}

@media (max-width: 600px) {

    .img-ope {
        height: 40vh;
    }
}
</style>

<!--
    <div style="width:60%" class="pt-5 pb-5">
                    <p style="font-weight: lighter;font-size:22px; font-weight: bold; color: #FFFFFF;">¿Cuándo debo acudir al consultorio del <a style="color:#2397D7">DR. ALEJANDRO MESARINA</a>?</p>
                    <p style="font-weight: lighter;font-size:20px; color: #FFFFFF;">Puedes acudir a nosotros por cualquier <a style="font-weight: bold ;color: #FFFFFF;">lesión o dolencia</a> que tengas <a style="color: #FFFFFF;font-weight: bold;">con tu sistema musculo-esquelético y articular</a>, de cualquier origen tanto <a style="color: #FFFFFF;font-weight: bold;">traumatico</a> como <a style="color: #FFFFFF;font-weight: bold; color: white;">degenerativo</a>, sea <a style="font-weight: bold; color: white;">por ejemplo para el tratamiento</a> de una lesión como es el caso de una <a style="font-weight: bold; color: white;">lesión de rodilla</a>, <a style="font-weight: bold; color: white;">cadera</a>, <a style="font-weight: bold; color:white;">tobillo</a>, <a style="font-weight: bold; color:white;">muñeca</a> o una dolencia de la <a style="font-weight: bold; color: white;">columna vertebral</a> o una condición desarrollada a lo largo del tiempo como <a style="font-weight: bold; color: white;">osteoartrosis</a>.</p>
                    <p style="font-weight: lighter;font-size:20px; color: #FFFFFF;"><a style="font-weight: bold; color: white;color: #FFFFFF;">Nuestro objetivo </a>es curar al íntegro la lesión que te aqueja, y en lesiones crónicas e irreversibles reducir el dolor, mejorar la movilidad y, sobre todo, la calidad de vida de nuestros pacientes.</p>
                </div>


<div style="display: flex; justify-content: center; align-items: center; flex: 4;">
                <v-img class="img-ope"></v-img>
            </div> 

-->