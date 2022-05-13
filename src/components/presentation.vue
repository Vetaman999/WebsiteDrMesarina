<template>
  <v-container>
        <v-card
          class=""
          max-width="100%"
        >
          <v-img
            class="white--text align-end"
            max-height="450px"
            src="../assets/Portada.png"
            color="transparent"
          >
          <v-conteiner grid-list-md>
            <v-layout row wrap>
              <v-flex>
                <v-card max-height="50px" color="transparent" elevation="0"></v-card>
                <v-div class="d-flex center"
                  width="100%"
                  style="
                    display: flex;
                    justify-content: center;
                    "
                >
                  <v-card max-width="280px" 
                    color="transparent"
                    elevation="0"
                    >
                    <v-img class="white--text align-end"
                      max-width="300px"
                      max-height="280px"
                      src="../assets/pres.png"
                    >
                    </v-img>
                  </v-card>
                  <v-card  max-width="10px" max-height="60px" color="transparent" elevation="0"></v-card>
                  <v-card color="transparent"
                    elevation="0"
                    max-width="1000px"
                  >
                    <v-card-title style="font-size:64px;
                      color:#FFFFFF;"
                    >
                      Dr. Alejandro Mesarina
                    </v-card-title>
                    <v-card-text style="font-size:20px; font-family: Arial; font-weight: lighter; color:#FFFFFF">
                      Médico doctorado en medicina y especialista en Cirugía Ortopédica
                    </v-card-text>
                    <v-card color="transparent" 
                      max-height="20%"
                      elevation="0"  
                    ></v-card>
                    <v-div class="d-flex center" style="
                      display: flex;
                      justify-content: center;"
                    >
                      <v-btn
                        style="background-color: #2397D7; 
                          color:#FFFFFF;
                          height: 55px;
                          max-width: 170px;
                          font-size: 18px;
                          font-family: sans-serif;
                          "
                      >
                        Contacto
                      </v-btn>
                    </v-div>
                  </v-card>
                </v-div>
                <v-card height="60" color="transparent" elevation="0"></v-card>
              </v-flex>
            </v-layout>
          </v-conteiner>
          </v-img>
        </v-card>
  </v-container>
</template>

<script>

  export default {
    name: 'presentation',
    data: () => ({

    }),
  }
</script>
<style>
</style>