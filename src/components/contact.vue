<template>
    <div>
        <div id="main-container" class="contact-container">
            <div class="contact-color-container first-color">
                <v-card color="transparent" elevation="0">
                    <v-card-text style="font-size:20px; font-weight: 200; color:white; letter-spacing: 0.05ch;">
                        Nos enfocamos en proporcionarle a nuestros pacientes tratamientos no quirúrgicos, no invasivos
                        y/o quirúrgicos que le permitan su recuperación, aliviar el dolor, rehabilitar y prevenir
                        futuras lesiones.
                    </v-card-text>
                    <v-card-actions>
                        <v-flex d-flex justify-start mt-15>
                            <v-btn to="/profile" style="background-color: #2397D7; color: white; height: 61px; width: 200px;">
                                <v-card-text style="font-size:20px; font-weight: lighter; color:#FFFFFF">
                                    CONOCER MÁS
                                </v-card-text>
                            </v-btn>
                        </v-flex>
                    </v-card-actions>
                </v-card>
            </div>
            <div id="second-color" class="contact-color-container second-color">
                <v-card color="transparent" elevation="0">
                    <v-card-text
                        style="font-size:20px; font-weight: 300; color:black; letter-spacing: 0.05ch; text-align: right;">
                        Pregúntanos sobre cualquier tema de nuestras especialidades o sobre lo que podemos hacer por ti.
                    </v-card-text>
                    <v-card-actions>
                        <v-flex d-flex justify-end mt-15>
                            <v-btn href="https://wa.me/947358498" target="_blank" style="background-color: #2397D7; color:#FFFFFF; height: 61px; width: 200px;">
                                <v-card-text class="justify-center d-flex" style="font-size:20px; font-weight: lighter; color: white">
                                    CONTACTAR
                                </v-card-text>
                            </v-btn>
                        </v-flex>
                    </v-card-actions>
                </v-card>
            </div>
        </div>
        <div id="ct-image" class="contact-image">
            <v-img src="../assets/microfno.png"></v-img>
        </div>
    </div>
</template>

<script>
export default {
    name: 'contact',
    data: () => ({
        mainContainerElement: null,
        colorElement: null,
        imageElement: null,
        imageOffset: {
            x: 20,
            y: 0
        }
    }),
    mounted() {
        this.mainContainerElement = document.getElementById("main-container");
        this.colorElement = document.getElementById("second-color");
        this.imageElement = document.getElementById("ct-image");

        window.addEventListener("resize", this.updateImagePosition);

        if (this.colorElement.offsetWidth == this.mainContainerElement.offsetWidth
            || this.mainContainerElement.offsetWidth < 400) {
            this.imageElement.style.visibility = "hidden";
            // this.imageElement.style.left = `${(this.mainContainerElement.offsetWidth / 2) - (this.imageElement.offsetWidth / 2)}px`;
            // this.imageElement.style.top = `${this.colorElement.offsetTop - (this.imageElement.offsetHeight / 2)}px`;
        }
        else {
            this.imageElement.style.visibility = "visible";
            this.imageElement.style.left = `${(this.colorElement.offsetWidth - (this.imageElement.offsetWidth / 2)) + this.imageOffset.x}px`;
            this.imageElement.style.top = `${(this.colorElement.offsetTop + (this.colorElement.offsetHeight / 2) - (this.imageElement.offsetHeight / 2)) + this.imageOffset.y + (this.imageElement.offsetHeight/8)}px`;            
        }
    },
    unmounted() {
        window.removeEventListener('resize', this.updateImagePosition);
    },
    methods: {

        updateImagePosition(e) {
            if (this.colorElement.offsetWidth == this.mainContainerElement.offsetWidth
                || this.mainContainerElement.offsetWidth < 400) {
                this.imageElement.style.visibility = "hidden";
                // this.imageElement.style.left = `${(this.mainContainerElement.offsetWidth / 2) - (this.imageElement.offsetWidth / 2)}px`;
                // this.imageElement.style.top = `${this.colorElement.offsetTop - (this.imageElement.offsetHeight / 2)}px`;
            }
            else {
                this.imageElement.style.visibility = "visible";
                this.imageElement.style.left = `${(this.colorElement.offsetWidth - (this.imageElement.offsetWidth / 2)) + this.imageOffset.x}px`;
                this.imageElement.style.top = `${(this.colorElement.offsetTop + (this.colorElement.offsetHeight / 2) - (this.imageElement.offsetHeight / 2)) + this.imageOffset.y + (this.imageElement.offsetHeight/8)}px`;            
            }
        }
    }
}
</script>

<style scoped>
.contact-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.contact-color-container {
    height: 450px;
    width: 49vw;
    flex-grow: 12;
    padding: 100px 5vw;
}

.first-color {
    background-color: #024F78;
}

.second-color {
    background-color: #CAE7F7;
}

.contact-image {
    width: 270px;
    height: 399.6px;
    position: absolute;
}

@media (max-width: 1000px) {
    .contact-color-container {
    width: 100vw;
    }

}

</style>







































        <!-- <v-flex xs12 sm6 d-flex align-content-center flex-wrap>
                    <v-img src="../assets/fon1.png" class="white--text align-center" height="100%">
                        <v-flex d-flex justify-center mb-6>
                            <v-card width="60%" height="60%" >
                                <v-card-text style="font-size:24px; font-weight: lighter; color:#FFFFFF">
                                    Nos enfocamos en proporcionarle a nuestros pacientes tratamientos no quirúrgicos, no invasivos y/o quirúrgicos que le permitan su recuperación, aliviar el dolor, rehabilitar y prevenir futuras lesiones.
                                </v-card-text>
                                <v-card-actions>
                                    <v-flex my-5 d-flex justify-start mb-6>
                                        <v-btn  style="background-color: #2397D7; color:#FFFFFF; height: 61px; width: 200px;">
                                            <v-card-text  style="font-size:24px; font-weight: lighter; color:#FFFFFF">
                                                PREGUNTANOS
                                            </v-card-text>
                                        </v-btn>
                                    </v-flex>
                                </v-card-actions>
                            </v-card>
                        </v-flex>
                    </v-img>
                </v-flex>
                <v-flex xs12 sm6 d-flex align-content-center flex-wrap>
                    <v-img src="../assets/fon2.png" class="align-center">
                        <v-flex d-flex justify-center mb-6>
                            <v-card width="60%" height="60%" >
                                <v-card-text style="font-size:24px; font-weight: lighter; color:black">
                                    Nos enfocamos en proporcionarle a nuestros pacientes tratamientos no quirúrgicos, no invasivos y/o quirúrgicos que le permitan su recuperación, aliviar el dolor, rehabilitar y prevenir futuras lesiones.
                                </v-card-text>
                                <v-card-actions>
                                    <v-flex my-5 d-flex justify-end mb-6>
                                        <v-btn  style="background-color: #2397D7; color:#FFFFFF; height: 61px; width: 200px;">
                                            <v-card-text  style="font-size:24px; font-weight: lighter; color:#FFFFFF">
                                                PREGUNTANOS
                                            </v-card-text>
                                        </v-btn>
                                    </v-flex>
                                </v-card-actions>
                            </v-card>
                        </v-flex>
                    </v-img>
                </v-flex> -->
        <!-- <v-flex xs12 sm6>    
                    <img src="../assets/microfno.png" style="position: absolute;  left: 43%; top:5px" width="300px">
                </v-flex> -->