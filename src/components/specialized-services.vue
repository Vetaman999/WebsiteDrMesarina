<template>
    <div style="margin:3%">
        <div style="display: flex; width: 100%; background-color: #E3F5FF; flex-wrap: wrap; ">

            <div
                style="display: flex; justify-content: center; align-items: center; height: 60vh; width: 500px;  flex: 4;">
                <v-carousel interval="3000" height="100%" id="base-doc-image" vertical cycle hide-delimiters :show-arrows="false">
                    <v-carousel-item v-for="(img, i) in imgs" :key="i" v-bind:src="img">
                    </v-carousel-item>
                </v-carousel>
            </div>
            <div style="display: flex; flex-direction: column; justify-content: center; align-items: center; flex: 9;">
                <div style="width:60%" class="pt-5 pb-5">
                    <p style="font-size:20px;">Este acercamiento de <a
                            style="font-weight: bold; color: black;">múltiples especialidades</a> nos permite <a
                            style="font-weight: bold; color: black;">proporcionar</a> a nuestros pacientes el acceso a
                        un <a style="font-weight: bold; color: black;">amplio rango</a> de <a
                            style="font-weight: bold; color: black;">servicios especializados</a> que incluyen:</p>
                    <ul type="*" style="font-size: 20px;">
                        <li>Evaluación integral y tratamiento relacionado con dolencias, desórdenes, enfermedades o
                            accidentes en general.</li>
                        <li>Evaluación Diagnostico y tratamiento de lesiones deportivas diversas.</li>
                        <li>Análisis de la dieta alimenticia y consejería nutricional.</li>
                        <li>Acceso al mejor equipo de especialistas en rehabilitación y terapia física.</li>
                        <li>Tratamiento integral de la persona (salud, estilo de vida, etapas del ciclo de vida, etc.).
                        </li>
                        <li>Médicos asociados en España y EE.UU.</li>
                        <li>Laboratorio especializado.</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import imgespe1 from '../assets/Fotos/IMG_1749.png'
import imgespe2 from '../assets/doctora.png'
import imgespe3 from '../assets/Fotos/IMG_1770.png'

export default {
    data: () => ({
        imgs: [
            imgespe1,
            imgespe2,
            imgespe3,

        ],
    }),
}
</script>
<style>
.img-chica {

    background: url('../assets/doctora.png') no-repeat;
    height: 60vh;
    background-size: cover;
    background-position: center;
    min-width: 300px;
}

@media (max-width: 400px) {

    .img {
        height: 40vh;
    }
}
</style>

<!--<div class="d-flex justify-start" style="align-items: center;flex-wrap: wrap">
        <div class="d-flex justify-end">
            <v-img height="700px" width="650px" src="../assets/doctora.png"></v-img>
        </div>
        <div style="width:1200px;border: 1px solid black;" class="d-flex justify-center">
            <div class="mx-auto mb-10" style="width: 50%;">
                <p style="font-size:22px;">Este acercamiento de <a>múltiples especialidades</a> nos permite <a>proporcionar</a> a nuestros pacientes el acceso a un <a>amplio rango</a> de <a>servicios especializados</a> que incluyen:</p>
                <ul type="*" style="font-size: 20px;">
                    <li>Evaluación integral y tratamiento relacionado con dolencias, desórdenes, enfermedades o accidentes en general.</li>
                    <li>Evaluación Diagnostico y tratamiento de lesiones deportivas diversas.</li>
                    <li>Análisis de la dieta alimenticia y consejería nutricional.</li>
                    <li>Acceso al mejor equipo de especialistas en rehabilitación y terapia física.</li>
                    <li>Tratamiento integral de la persona (salud, estilo de vida, etapas del ciclo de vida, etc.).</li>
                    <li>Médicos asociados en España y EE.UU.</li>
                    <li>Laboratorio especializado.</li>
                </ul>
                <div class="d-flex justify-center">
                    <v-btn style="background-color: #2397D7; color: white; height: 50px; width: 200px;">
                        <v-card-text style="font-size:20px; font-weight: lighter; color:#FFFFFF">
                            CONTACTO
                        </v-card-text>
                    </v-btn>
                </div>
            </div>
        </div>        
    </div>-->