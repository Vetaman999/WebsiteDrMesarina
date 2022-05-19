<template>
    <div style="display: flex; width: 100%; background-color: #CAE7F7; flex-wrap: wrap;">
        <div style="display: flex; flex-direction: column; justify-content: center; align-items: center; flex: 9;">
            <div style="width:90%" class="pt-5 pb-5">
                <p style="font-size:22px; font-weight: bold;">¿Cuándo debo acudir al consultorio del <a style="color:#2397D7">DR. ALEJANDRO MESARINA</a>?</p>
                <p style="font-size:17px;">Puedes acudir a nosotros por cualquier <a style="font-weight: bold; color: black;">lesión o dolencia</a> que tengas <a style="font-weight: bold; color: black;">con tu sistema musculo-esquelético y articular</a>, de cualquier origen tanto <a style="font-weight: bold; color: black;">traumatico</a> como <a style="font-weight: bold; color: black;">degenerativo</a>, sea <a style="font-weight: bold; color: black;">por ejemplo para el tratamiento</a> de una lesión como es el caso de una <a style="font-weight: bold; color: black;">lesión de rodilla</a>, <a style="font-weight: bold; color: black;">cadera</a>, <a style="font-weight: bold; color: black;">tobillo</a>, <a style="font-weight: bold; color: black;">muñeca</a> o una dolencia de la <a style="font-weight: bold; color: black;">columna vertebral</a> o una condición desarrollada a lo largo del tiempo como <a style="font-weight: bold; color: black;">osteoartrosis</a>.</p>
                <p style="font-size:17px;"><a style="font-weight: bold; color: black;">Nuestro objetivo </a>es curar al íntegro la lesión que te aqueja, y en lesiones crónicas e irreversibles reducir el dolor, mejorar la movilidad y, sobre todo, la calidad de vida de nuestros pacientes.</p>
            </div>
        </div>
        <div style="display: flex; justify-content: center; align-items: center; flex: 4;">
            <v-img class="img-ope"></v-img>
        </div>        
    </div>
</template>

<style scoped>

.img-ope {
    
    background: url('../assets/ope.png') no-repeat;
    height: 60vh;
    background-size: cover;
    background-position: center;
    min-width: 300px;
}

@media (max-width: 600px) {

  .img{
    height: 40vh;
  }
}
</style>