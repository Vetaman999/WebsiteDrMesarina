<template>
  <v-card
    class=""
    max-width="100%"
    flex
    
  >
    <v-img
      class="white--text align-end"
      height="450px"
      src="../assets/Portada.png"
      color="transparent"
    >
      <v-card height="50px" color="transparent" elevation="0"></v-card>
      <div class="d-flex center"
        width="100%"
        style="
          display: flex;
          justify-content: center;
          "
      >
        <v-card width="280px" 
          color="transparent"
          elevation="0"
          >
          <v-img class="white--text align-end"
            width="300px"
            height="280px"
            src="../assets/pres.png"
          >
          </v-img>
        </v-card>
        <v-card  width="10px" height="60" color="transparent" elevation="0"></v-card>
        <v-card color="transparent"
          elevation="0"
          width="34%"
        >
          <a
            style="font-size:64px;
            color:#FFFFFF;"
          >
            Dr. Alejandro Mesarina
          </a>
          <a 
            style="font-size:20px; 
              font-family: Arial; 
              font-weight: lighter;
              color:#FFFFFF"
          >
            Médico doctorado en medicina y especialista en Cirugía Ortopédica
          </a>
          <v-card color="transparent" 
            height="20%"
            elevation="0"  
          ></v-card>
          <div class="d-flex center" style="
            display: flex;
            justify-content: center;"
          >
            <v-btn
              style="background-color: #2397D7; 
                color:#FFFFFF;
                height: 55px;
                width: 170px;
                font-size: 18px;
                font-family: sans-serif;
                "
            >
              Contacto
            </v-btn>
          </div>
        </v-card>
      </div>
      <v-card height="60" color="transparent" elevation="0"></v-card>
    </v-img>
  </v-card>
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