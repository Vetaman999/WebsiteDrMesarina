<template>
    <div class="presentation-carousel">
        <v-carousel interval="9000" cycle v-model="model" hide-delimiter-background height="100%">
            <v-carousel-item v-for="(img, i) in imgs" :key="i" v-bind:src="img">
            </v-carousel-item>
            <div style="z-index: 1; position:absolute; width: 100%; height: 100%; ">
                <div class="presentation-container">
                    <div style="height: fit-content; width: fit-content;">
                        <img class="presentation-img" src="../assets/pres.png" />
                    </div>

                    <div class="presentation-text-container">
                        <div class="presentation-title">Dr. Alejandro Mesarina</div>
                        <div class="presentation-description">Médico doctorado en medicina y especialista en cirugía
                            ortopédica</div>
                        <v-btn
                            style="background-color: #2397D7; color: #FFFFFF; height: 61px; width: 200px; font-size:24px; font-weight: 300; align-self: center; margin-top: 30px;"
                            href="https://wa.me/996999489" target="_blank">Contacto</v-btn>
                    </div>
                </div>
            </div>
        </v-carousel>
    </div>
</template>

<script>
import imgportada1 from "../assets/portada1.png"
import imgportada2 from "../assets/portada2.png"
import imgportada3 from "../assets/portada3.png"
import imgportada4 from "../assets/portada4.png"

export default {
    data: () => ({
        DrAlejandroMesarina: 96448717,
        model: 0,
        imgs: [
            imgportada1,
            imgportada2,
            imgportada3,
            imgportada4,
        ],
    }),
}
</script>

<style scoped>
.presentation-carousel {
    height: 30vw;
}

.presentation-container {
    height: 100%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;

}

.presentation-text-container {  
    height: fit-content;
    display: flex;
    flex-direction: column;
    margin-left: 30px;
}

.presentation-title {
    font-size: 4vw;
    font-weight: 500;
    color: white;
}

.presentation-img{
    width:300px; height:300px;
}
.presentation-description {
    margin-top: -24px;
    font-size: 1.7vw;
    font-weight: 150;
    color: white;
}

                            
@media (max-width: 1000px) {
    .presentation-img{
        height: 270px;
        width: 270px;
    }
    .presentation-carousel {
        height: 220vh;
    }

    .presentation-container {
        height: 90%;
    }

    .presentation-text-container {
        margin-left: 0;
    }

    .presentation-title {
        font-size: 6vw;
    }

    .presentation-description {
        font-size: 3vw;
    }

}

@media (max-width: 700px) {
    .presentation-img{
        margin-top: 20px;
        height: 220px;
        width: 220px;
    }
    .presentation-text-container {
        margin: 0 20px;
        justify-content: center;
    }

    .presentation-title {
        font-size: 8vw;
        text-align: center;
    }

    .presentation-description {
        font-size: 5vw;
        text-align: center;
    }
}
</style>