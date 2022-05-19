<template>
  <section class="main_container">

    <div class="treatments">
      <div class="left_box">
        <h4>TRATAMIENTO ORTOPÉDICO NO QUIRÚRGICO</h4>
        <p>No todos los problemas ortopédicos requieren de cirugía. Para muchas condiciones, la medicina regenerativa y/o correctiva proporciona una alternativa para aquellos que buscan evitar la cirugía o que desean prolongar la necesidad de una operación o que no pueden ser candidatos a una.</p>
        <v-list class="list_box">
            <v-list-group
                v-for="item in items"
                :key="item.title"
                v-model="item.active"
            >
              <template v-slot:activator>
                <v-list-item-content>
                  <v-list-item-title v-text="item.title"></v-list-item-title>
                </v-list-item-content>
              </template>

              <v-list-item
                  v-for="child in item.items"
                  :key="child.title"
              >
                <v-list-item-content>
                  <v-list-item-title v-text="child.title"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-group>
          </v-list>
      </div>
      <div class="img_1"></div>
      <div class="img_2"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "treatments",
  data: () => ({
    items: [
      {
        items: [{ title: 'List Item' }],
        title: 'Viscosuplementación',
      },
      {
        items: [
          { title: 'Breakfast & brunch' },
          { title: 'New American' },
          { title: 'Sushi' },
        ],
        title: 'Suero autólogo condicionado',
      },
      {
        items: [{ title: 'List Item' }],
        title: 'Terapia con células madre',
      },
      {
        items: [{ title: 'List Item' }],
        title: 'Terapia física y rehabilitación',
      },
      {
        items: [{ title: 'List Item' }],
        title: 'Nutrición',
      },
    ],
  })
}
</script>

<style scoped>
.main_container{
  padding: 1rem;
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
.title h2{
  color: #2397D7;
}
hr{
  width: 82%;
  height: 2px;
  background-color: #6789a1;
  border: #6789a1;
}

.treatments{
  width: 100%;
  padding: 2rem 4rem;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap: 2rem 6rem;
  grid-template-areas:
  "left_box img1"
  "left_box img2";
}

.left_box{
  grid-area: left_box;
}
.left_box h4, .left_box p, .left_box .list_box{
  margin-bottom: 1.5rem;
}
.img_1{
  grid-area: img1;
  background: url('../assets/treatments_img1.jpg') no-repeat;
}
.img_2{
  grid-area: img2;
  background: url('../assets/treatments_img2.jpg') no-repeat;
}
.img_1, .img_2{
  height: 40vh;
  background-size: cover;
  background-position: center;
  border-radius: 1rem;
}

@media (max-width: 850px) {
  .treatments{
    height: 120vh;
    padding: 2rem 0.5rem;
    grid-template-areas:
    "left_box left_box"
    "img1 img2";
    gap: 1rem;
  }
}
@media (max-width: 560px) {
  .treatments{
    padding: 2rem 0;
    height: 108vh;
  }
  .img_1, .img_2{
    height: 20vh;
  }
}
</style>