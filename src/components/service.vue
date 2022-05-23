<template>
    <v-card elevation="0" color="transparent" style="margin: auto 0">
        <v-container grid-list-md>
            <v-layout row wrap>
                <v-card width="200px" class="mx-auto" elevation="0" color="transparent">
                    <v-img class="mx-auto" src="../assets/icon2.png" width="77px" height="77px"></v-img>
                    <div :class="anime">
                        <v-card-title class="justify-center"
                            style="margin-top: 10px;font-size:80px; font-weight: medium; color:#024F78">100
                        </v-card-title>

                        <v-card-subtitle class="d-flex justify-center"
                            style="margin-top: 10px;font-size:20px; font-weight: medium; color:black">Pacientes Leales
                        </v-card-subtitle>
                    </div>
                </v-card>
                <v-card width="200px" class="mx-auto" elevation="0" color="transparent">
                    <v-img class="mx-auto" src="../assets/icon1.png" width="77px" height="77px"></v-img>
                    <div class="anima">
                        <v-card-title class="justify-center"
                            style="margin-top: 10px;font-size:80px; font-weight: medium; color:#024F78">30
                        </v-card-title>
                        <v-card-subtitle class="d-flex justify-center"
                            style="margin-top: 10px;font-size:20px; font-weight: medium; color:black">Experiencia
                        </v-card-subtitle>
                    </div>
                </v-card>
                <v-card width="200px" class="mx-auto" elevation="0" color="transparent">
                    <v-img class="mx-auto" src="../assets/icon 2.png" width="77px" height="77px"></v-img>
                    <div class="anima">
                        <v-card-title class="justify-center"
                            style="margin-top: 10px;font-size:80px; font-weight: medium; color:#024F78">10
                        </v-card-title>
                        <v-card-subtitle class="d-flex justify-center"
                            style="margin-top: 10px;font-size:20px; font-weight: medium; color:black">Especialidades
                        </v-card-subtitle>
                    </div>
                </v-card>
                <v-card width="200px" class="mx-auto" elevation="0" color="transparent">
                    <v-img class="mx-auto" src="../assets/icon4.png" width="77px" height="77px"></v-img>
                    <div class="anima">
                        <v-card-title class="justify-center"
                            style="margin-top: 10px;font-size:80px; font-weight: medium; color:#024F78">40
                        </v-card-title>
                        <v-card-subtitle class="d-flex justify-center"
                            style="margin-top: 10px;font-size:20px; font-weight: medium; color:black">Tratamientos
                        </v-card-subtitle>
                    </div>
                </v-card>
            </v-layout>
        </v-container>
    </v-card>
</template>

<style scoped>
</style>

<!--
    .anima{
    animation-name: animate;
    animation-duration: 3s;
    position: relative;
    animation-iteration-count: infinite;
}

@keyframes animate {
    0% {
        opacity: 40%;
    }

    25% {
        opacity: 70%;
    }

    50% {
        opacity: 100%;
    }

    75% {
        opacity: 70%;
    }

    100% {
        opacity: 40%;
    }
}
-->