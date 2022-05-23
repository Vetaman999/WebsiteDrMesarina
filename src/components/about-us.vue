<template>
  <section class="main_container">
    <div class="left_box">
      <v-carousel id="base-doc-image" style="width: 83%; height: 60vh;" cycle hide-delimiters :show-arrows="false">
        <v-carousel-item v-for="(img) in imgs" :key="img" v-bind:src="img"></v-carousel-item>
      </v-carousel>
      <div id="doc-image" class="doc-image">
        <v-img height="100%" src="../assets/doc1.png"></v-img>
      </div>
    </div>

    <div class="right_box py-10">
      <h1 class="title_dr" style="font-size:4vh">Dr. Mesarina</h1>
      <h3 style="font-size:2.5vh; ">¿Porqué acudir con nosotros?</h3>
      <hr class="mb-10 mt-4">
      <p style="font-size:20px;">Nuestro objetivo es curar ad íntegro la lesión que te aqueja, y en lesiones crónicas e
        irreversibles reducir el dolor, mejorar la movilidad y, sobre todo, la calidad de vida de nuestros pacientes.
      </p>
      <v-btn class="mt-10" style=";background-color: #2397D7; color: white; height: 59px; width: 200px;" to="/profile">
                <v-card-text class=" my-auto justify-center d-flex" style=";font-size:20px; font-weight: lighter; color:#FFFFFF">
                    Conocenos
                </v-card-text>
      </v-btn>
    </div>
  </section>
</template>

<script>
import imgabout1 from "../assets/about-img.png"
import imgabout2 from "../assets/cor.jpg"
import imgabout3 from "../assets/IMG_1771.png"

export default {
  name: "about-us",
  data: () => ({
    baseImageElement: null,
    imageElement: null,
    imgs: [
      imgabout1,
      imgabout2,
      imgabout3,
    ],
  }),

  mounted() {
    this.baseImageElement = document.getElementById("base-doc-image");
    this.imageElement = document.getElementById("doc-image");

    window.addEventListener("resize", this.updateImagePosition);

    this.imageElement.style.left = `${this.baseImageElement.offsetLeft + this.baseImageElement.offsetWidth - (this.imageElement.offsetWidth / 2)}px`;
    this.imageElement.style.top = `${this.baseImageElement.offsetTop + (this.baseImageElement.offsetHeight) - (this.imageElement.offsetHeight + 200)}px`;
  },
  unmounted() {
    window.removeEventListener('resize', this.updateImagePosition);
  },
  methods: {

    updateImagePosition(e) {
      this.imageElement.style.left = `${this.baseImageElement.offsetLeft + this.baseImageElement.offsetWidth - (this.imageElement.offsetWidth / 2)}px`;
      this.imageElement.style.top = `${this.baseImageElement.offsetTop + this.baseImageElement.offsetHeight - (this.imageElement.offsetHeight / 2)}px`;
    }
  }
}
</script>

<style scoped>
.doc-image {
  width: 200px;
  height: 12%;
  position: absolute;
  box-shadow: 0 0 15px 2px black;
}

.main_container {
  margin-top: 50px;
  display: flex;
  justify-content: space-evenly;
  height: 60vh;
}

.left_box {
  width: 50%;
}

.right_box {
  width: 40%;
  display: flex;
  flex-direction: column;
}

.right_box * {
  margin-bottom: 1rem;
}

.title_dr {
  font-size: 3rem;
  color: #054c73;
}

hr {
  width: 20%;
  background-color: #5b5b5b;
  height: 3px;
}

@media (max-width: 695px) {
  .main_container {
    height: 100vh;
    flex-direction: column;
    align-items: center;
  }

  .left_box,
  .right_box {
    width: 90%;
  }
}
</style> 