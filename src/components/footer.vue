<template>
  <section class="img_bg">
    <div class="blue_filter">
      <div class="left_box">
        <img class="img_doc" src="https://i2.wp.com/doctormesarina.com/wp-content/uploads/2018/09/dr-mesarina-logo-footer.png?resize=300%2C32&ssl=1" alt="doc">
        <p class="act_call text_p">
          Estamos convencidos que para mantener un estilo de vida saludable y evitar el deterioro de otros órganos y funciones de estos debemos mantenernos activos y, por esta razón, hacemos todo lo que s encuentre en nuestras manos para que nuestros pacientes regresen a sus actividades diarias y deportivas.
        </p>
      </div>
      <hr>
      <div class="right_box">
        <h3 class="text_p">ESTAMOS EN:</h3>
        <div class="sec">
          <div class="sec_one">
            <v-icon dark>place</v-icon>
            <p class="text_p">Calle Monterrey 355 of. 903, Chacarilla del Estanque, Surco, Lima.</p>
          </div>
          <div class="sec_one">
            <v-icon dark>whatsapp</v-icon>
            <p class="text_p">947 358 498</p>
          </div>
          <div class="sec_one">
            <v-icon dark>phone</v-icon>
            <p class="text_p">200 2270</p>
          </div>
          <div class="sec_email">
            <v-icon dark>mail_outline</v-icon>
            <p class="text_p">drmesarina@doctormesarina.com
              endocrinologia@doctormesarina.com
              nutricion@doctormesarina.com
              fisioterapia@doctormesarina.com
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "footer"
}
</script>

<style scoped>
.text_p{
  color: #eeeeee;
  font-size:20px; 
  font-weight: lighter
}
.img_bg {
  background: url('../assets/foot.png') no-repeat;
  width: 100%;
  height: 45vh;
  background-size: cover;
  background-position: center;
  position: relative;
}
.blue_filter{
  background: rgba(0, 50, 78, 0.9);
  height: 100%;
  display: flex;
  align-items: center;
}
.left_box{
  height: 100%;
  width: 50%;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
}
.img_doc {
  width: 50%;
}
.act_call {
  width: 75%;
}
hr{
  height: 70%;
}
.right_box{
  height: 100%;
  width: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
}
.sec{
  width: 75%;
}
.sec_one{
  display: flex;
  align-items: center;
  justify-content: center;
  width: fit-content;
}
.sec_one p {
  margin: 8px;
}
.sec_email{
  display: flex;
  justify-content: space-evenly;
  width: fit-content;
}
.sec_email p{
  margin-left: 10px;
}
@media (max-width: 1076px){
  .img_bg{
    height: 90vh;
  }
  .blue_filter{
    flex-direction: column;
  }
  .img_doc {
    width: 30%;
  }
  hr{
    height: 1px;
    width: 70%;
  }
  .left_box{
    width: 100%;
  }
  .right_box{
    width: 100%;
  }
  .sec_email{
    justify-content: start;
    width: 100%;
  }
  .sec_email p{
    width: 40%;
  }
}
@media (max-width: 728px){
  .sec_email p{
    margin-right: 4rem;
  }
}
@media (max-width: 558px){
  .sec{
    width: 100%;
    padding: 1rem;
  }
  .sec_email p{
    margin-right: 3rem;
  }
}

</style>