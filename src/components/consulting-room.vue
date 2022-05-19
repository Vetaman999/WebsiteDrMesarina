<template>
<div style="margin:3%;">
    <div style="display: flex; width: 100%; background-color: #005483; flex-wrap: wrap;">
        <div style="display: flex; flex-direction: column; justify-content: center; align-items: center; flex: 9;">
            <div style="width:60%" class="pt-5 pb-5">
                <p style="font-size:22px; font-weight: bold; color: white;">Dependiendo de las necesidades de nuestros pacientes, nuestro consultorio incluye:</p>
                <ul type="*" style="font-size: 20px;font-weight: lighter; color: white;">
                    <li>Diagnóstico</li>
                    <li>Tratamientos no invasivos, conservadores no quirúrgicos.</li>
                    <li>Tratamientos Quirúrgicos Ortopédicos de toda magnitud como Artroscopías de Articulaciones tipo rodilla, hombro, cadera, tobillo a fin de reparar lesiones articulares de diversa etiologia.</li>
                    <li>Tratamientos Quirúrgicos de reemplazo articulares, prótesis totales y parciales de rodillas y cadera.</li>
                    <li>Medicina deportiva, curación de lesiones propias al deporte a fin de restablecer las funciones de máximo rendimiento, asimismo contamos con asesoramiento, coaching, psicología deportiva.</li>
                    <li>Terapia física y rehabilitación</li>
                    <li>Nutrición para el alto rendimiento</li>
                    <li>Asesoramiento para alcanzar metas deportivas y/o de optimo función articular</li>
                    <li>Medicina familiar</li>
                </ul>
            </div>
        </div>
        <div style="display: flex; justify-content: center; align-items: center; flex: 4;">
            <v-img class="img-diploma"></v-img>
        </div>        
    </div>
</div>
</template>
<style>
.img-diploma {
    
    background: url('../assets/diploma.png') no-repeat;
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
