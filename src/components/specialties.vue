<template>
  <section class="main_container">
    <div class="specialties">
      <div class="left_box">
        <h4>Dentro de nuestras especialidades se encuentran:</h4>
        <ul>
          <li>El tratamiento de dolencias y lesiones de rodillas, como meniscopatías,sutura de meniscos incluyendo reconstrucción de ligamentos, regeneración de articulaciones, artroscopias, prótesis, etc.</li>
          <li>El diagnóstico o tratamiento de problemas y lesiones del pie y tobillo tanto ligamentaria como osea o funcional.</li>
          <li>El tratamiento de condiciones relacionadas con las manos y la muñeca, incluyendo la reconstrucción.</li>
          <li>El cuidado completo de la cadera lesiones de cartilago, oseas y ligamentarias.</li>
          <li>El tratamiento de tendones y músculos, fracturas y reparaciones y reconstrucción del hombro y codo.</li>
          <li>La intervención no invasiva para reducir el dolor y restauración de la función de la columna vertebral.</li>
          <li>El tratamiento quirúrgico y no quirúrgico de fracturas y huesos rotos que no se curan o que se curan incorrectamente.</li>
          <li>La prevención y rehabilitación de condiciones relacionadas con el deporte en adolescentes y adultos.</li>
          <li>El tratamiento y cuidado de desórdenes y enfermedades ortopédicas pediátricas.</li>
          <li>El mejoramiento de la salud y tratamiento de osteoporosis.</li>
        </ul>
      </div>

      <div class="img"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "specialties"
}
</script>

<style scoped>
.main_container{
  padding: 1rem;
  background-color: #CAE7F7;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.title{
  width: 90%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
hr{
  width: 82%;
  height: 2px;
  background-color: #6789a1;
  border: #6789a1;
}

.specialties{
  padding: 1rem 0;
  width: 90%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.left_box{
  width: 60%;
}
.left_box h4{
  margin-bottom: 0.5rem;
}
.img{
  background: url('../assets/specialties_img.jpg') no-repeat;
  width: 35%;
  height: 40vh;
  background-size: cover;
  background-position: center;
  border-radius: 2rem;
}
@media (max-width: 900px){
  hr{
    width: 60%;
  }
  .specialties{
    width: 100%;
    flex-direction: column;
  }
  .left_box{
    width: 90%;
  }
  .img{
    margin: 2rem;
    width: 60%;
  }
}
@media (max-width: 520px) {
  hr{
    width: 40%;
  }
  .img{
    width: 80%;
    border-radius: 1rem;
  }
}
</style>