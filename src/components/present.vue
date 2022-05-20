<template>
    <div class="presentation-carousel">
        <v-carousel v-model="model" hide-delimiter-background height="100%">
            <v-carousel-item v-for="(img, i) in imgs" :key="i" v-bind:src="img">
                <!-- <v-container grid-list-md fill-height fluid>
                            <v-flex xs12 sm4 d-flex justify-end mb-6>
                                <v-card color="transparent" elevation="0">
                                    <v-img src="../assets/pres.png" max-height="350px" max-width="350px" d-flex></v-img>
                                </v-card>
                            </v-flex>
                            <v-flex d-flex align-content-center flex-wrap>    
                                <v-card d-flex  color="transparent" elevation="0">
                                    <v-card-title mb-7 style="font-size:5vw; color:#FFFFFF;">
                                        Dr.Alejandro Mesarina
                                    </v-card-title>
                                    <v-card-text style="margin-top: 30px;font-size:1.5vw; ; font-weight: lighter; color:#FFFFFF">
                                        Médico doctorado en medicina y especialista en Cirugía Ortopédica
                                    </v-card-text>
                                    <v-card-actions>
                                        <v-flex my-5 d-flex justify-center mb-6>
                                            <v-btn href="https://wa.me/996999489" class="d-flex justify-center" target="_blank" style=";background-color: #2397D7; color:#FFFFFF; height: 61px; width: 200px;">
                                                <v-card-text  style="font-size:24px; font-weight: lighter; color:#FFFFFF">
                                                    Contacto
                                                </v-card-text>
                                            </v-btn>
                                        </v-flex>
                                    </v-card-actions>
                                </v-card>
                            </v-flex>
                    </v-container> -->
                <div class="presentation-container">
                    <div style="height: fit-content;">
                        <v-img src="../assets/pres.png" width="300px" height="300px" />
                    </div>

                    <div class="presentation-text-container">
                        <div class="presentation-title">Dr. Alejandro Mesarina</div>
                        <div class="presentation-description">Médico doctorado en medicina y especialista en cirugía
                            ortopédica</div>
                        <v-btn
                            style="background-color: #2397D7; color: #FFFFFF; height: 61px; width: 200px; font-size:24px; font-weight: 300; align-self: center; margin-top: 30px;"
                            href="https://wa.me/996999489" target="_blank">Contacto</v-btn>
                    </div>
                </div>
            </v-carousel-item>
        </v-carousel>
    </div>
</template>

<script>
import Portada from "../assets/Portada.png"

export default {
    data: () => ({
        DrAlejandroMesarina: 96448717,
        model: 0,
        imgs: [
            Portada,
            Portada,
            Portada,
            Portada,
        ],
    }),
}
</script>

<style scoped>
.presentation-carousel {
    height: 30vw;
}

.presentation-container {
    height: 100%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}

.presentation-text-container {
    height: fit-content;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-left: 30px;
}

.presentation-title {
    font-size: 5vw;
    font-weight: 500;
    color: white;
}

.presentation-description {
    font-size: 2vw;
    font-weight: 200;
    color: white;
}

@media (max-width: 1000px) {
    .presentation-carousel {
        height: 650px;
    }

    .presentation-container {
        height: 90%;
    }
    .presentation-text-container{
        margin-left: 0;
    }

    .presentation-title {
        font-size: 6vw;
    }

    .presentation-description {
        font-size: 3vw;
    }

}

@media (max-width: 700px) {
    .presentation-text-container{
        margin: 0 20px;
        justify-content: center;
    }
    .presentation-title {
        font-size: 8vw;
        text-align: center;
    }

    .presentation-description {
        font-size: 5vw;
        text-align: center;
    }
}
</style>