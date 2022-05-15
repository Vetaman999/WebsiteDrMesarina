<template>
  <section class="main_container">
    <div class="left_box">
      <div class="img_bg">
        <div class="blue_filter">
        </div>
      </div>
      <img src="" alt="">
    </div>
    <div class="right_box">
      <h1 class="title_dr">Dr. Mesarina</h1>
      <h3>¿Porqué acudir con nosotros?</h3>
      <hr>
      <p>Nuestro objetivo es curar ad íntegro la lesión que te aqueja, y en lesiones crónicas e irreversibles reducir el dolor, mejorar la movilidad y, sobre todo, la calidad de vida de nuestros pacientes.</p>
      <v-btn style="background-color: #2397D7; width: fit-content" dark>Conocenos</v-btn>
    </div>
  </section>
</template>

<script>
export default {
  name: "about-us"
}
</script>

<style scoped>
.main_container{
  margin-top: 50px;
  display: flex;
  justify-content: space-evenly;
  height: 50vh;
}
.img_bg {
  background: url('../assets/about-img.png')no-repeat;
  width: 80%;
  height: 50vh;
  background-size: cover;
  background-position: center;

}
.left_box {
  width: 50%;
}
.right_box{
  width: 40%;
  display: flex;
  flex-direction: column;
}
.right_box * {
  margin-bottom: 1rem;
}
.title_dr{
  font-size: 3rem;
  color: #054c73;
}
hr{
  width: 20%;
  background-color: #5b5b5b;
  height: 3px;
}
@media (max-width: 695px){
  .main_container {
    height: 100vh;
    flex-direction: column;
    align-items: center;
  }
  .left_box, .right_box{
    width: 90%;
  }
}
</style>