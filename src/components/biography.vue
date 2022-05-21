<template>
    <div style="margin:3%;">
        <div style="display: flex; width: 100%; background-color: #CAE7F7; flex-wrap: wrap;">
            <div style="display: flex; flex-direction: column; justify-content: center; align-items: center; flex: 9;">
                <div style="width:60%" class="pt-5 pb-5">
                    <p style="font-size:17px;">El <a style="font-weight: bold; color: #2397D7;">Dr. Alejandro
                            Mesarina</a> es médico doctorado en medicina y <a
                            style="font-weight: bold; color: black;">especialista</a> en <a
                            style="font-weight: bold; color: black;">Cirugía Ortopédica</a>, graduado como tal en el
                        Hospital <a style="font-weight: bold; color: black;">Universitario Balgrist Zurich Suiza</a>. En
                        nuestro consultorio, junto a su equipo integrado de especialistas, nos permite llegar a <a
                            style="font-weight: bold; color: black;">diagnósticos certeros</a>, así como proponer las <a
                            style="font-weight: bold; color: black;">más modernas</a> y variadas posibilidades de
                        tratamiento.</p>
                    <p style="font-size:17px;">Asimismo, nos enfocamos en la <a
                            style="font-weight: bold; color: black;">prevención</a> y <a
                            style="font-weight: bold; color: black;">rehabilitación</a> de dolencias, desórdenes y
                        enfermedades del <a style="font-weight: bold; color: black;">sistema músculo-esquelético y
                            articular</a>, el cual incluye huesos, articulaciones, ligamentos, músculos, nervios y
                        tendones.</p>
                    <p style="font-size:17px;">Impulsamos el cuidado <a
                            style="font-weight: bold; color: black;">preventivo</a> mediante la promoción de la salud,
                        el bienestar, la actividad física y el aumento del desempeño físico <a
                            style="font-weight: bold; color: black;">bajo estrictos estándares médicos.</a></p>
                    <div class="d-flex justify-center">
                        <v-btn style="background-color: #2397D7; color: white; height: 61px; width: 310px;">
                            <v-card-text style="font-size:20px; font-weight: lighter; color:#FFFFFF">
                                CONTACTO
                            </v-card-text>
                        </v-btn>
                    </div>
                </div>
            </div>
            <v-hover v-slot="{ hover }">
                <div style="display: flex; justify-content: center; align-items: center; flex: 4;">
                    <v-img class="img-bio">
                        <v-expand-transition>
                            <div v-if="hover"
                                style="display: flex; justify-content: center; align-items: center; flex: 4;">
                                <v-img class="img-bio2"></v-img>
                            </div>
                        </v-expand-transition>
                    </v-img>
                </div>
            </v-hover>
        </div>
    </div>
</template>
<style>
.img-bio {
    background: url('../assets/Fotos/IMG_1753.png') no-repeat;
    height: 70vh;
    background-size: cover;
    background-position: center;
    min-width: 300px;
}
.img-bio2 {
    background: url('../assets/Fotos/IMG_1756.png') no-repeat;
    height: 70vh;
    background-size: cover;
    background-position: center;
    min-width: 300px;
}

@media (max-width: 600px) {

    .img {
        height: 40vh;
    }
}
</style>
