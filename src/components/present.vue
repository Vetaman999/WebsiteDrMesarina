<template>
    <v-card>
        <v-img class="white--text align-center" height="600px" src="../assets/Portada.png">
            <v-container grid-list-md fill-height fluid>
                    <v-flex xs12 sm4 d-flex justify-end mb-6>
                        <v-card color="transparent" elevation="0">
                            <v-img src="../assets/pres.png" max-height="350px" max-width="350px" d-flex></v-img>
                        </v-card>
                    </v-flex>
                    <v-flex d-flex align-content-center flex-wrap>    
                        <v-card d-flex  color="transparent" elevation="0">
                            <v-card-title mb-7 style="font-size:75px; color:#FFFFFF;">
                                Dr.Alejandro Mesarina
                            </v-card-title>
                            <v-card-text style="margin-top: 10px;font-size:23.5px; ; font-weight: lighter; color:#FFFFFF">
                                Médico doctorado en medicina y especialista en Cirugía Ortopédica
                            </v-card-text>
                            <v-card-actions>
                                <v-flex my-5 d-flex justify-center mb-6>
                                    <v-btn style="background-color: #2397D7; color:#FFFFFF; height: 61px; width: 200px;">
                                        <v-card-text  style="font-size:24px; font-weight: lighter; color:#FFFFFF">
                                            Contacto
                                        </v-card-text>
                                    </v-btn>
                                </v-flex>
                            </v-card-actions>
                        </v-card>
                    </v-flex>
            </v-container>
        </v-img>
    </v-card>