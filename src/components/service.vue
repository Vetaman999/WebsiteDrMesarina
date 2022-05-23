<template>
    <v-card elevation="0" color="transparent" style="margin: auto 0">
        <v-container grid-list-md>
            <v-layout row wrap>
                <v-card width="200px" class="mx-auto" elevation="0" color="transparent">
                    <v-img class="mx-auto" src="../assets/icon2.png" width="77px" height="77px"></v-img>
                    <div id="anima">
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
                    <div id="anima2">
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
                    <div id="anima3">
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
                    <div id="anima4">
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

<style>
#anima,
#anima2,
#anima3,
#anima4 {
    animation-name: animate;
    animation-duration: 5s;
    position: relative;     
    animation-iteration-count: infinite;
}

@keyframes animate {
    0% {
        opacity: 20%;
    }

    25% {
        opacity: 25%;
    }

    50% {
        opacity: 50%;
    }

    75% {
        opacity: 75%;
    }

    100% {
        opacity: 100%;
    }
}
</style>