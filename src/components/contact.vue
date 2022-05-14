<template>
    <div>
        <div id="main-container" class="contact-container">
            <div class="contact-color-container first-color"></div>
            <div id="second-color" class="contact-color-container second-color"></div>
        </div>
        <div id="image" class="contact-image">
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
        imageElement: null
    }),
    mounted() {
        this.mainContainerElement = document.getElementById("main-container");
        this.colorElement = document.getElementById("second-color");
        this.imageElement = document.getElementById("image");

        window.addEventListener("resize", this.updateImagePosition);

        if (this.colorElement.offsetWidth == this.mainContainerElement.offsetWidth
            || this.mainContainerElement.offsetWidth < 400) {
            this.imageElement.style.left = `${(this.mainContainerElement.offsetWidth / 2) - (this.imageElement.offsetWidth / 2)}px`;
            this.imageElement.style.top = `${this.colorElement.offsetTop - (this.imageElement.offsetHeight / 2)}px`
        }
        else {
            this.imageElement.style.left = `${this.colorElement.offsetWidth - (this.imageElement.offsetWidth / 2)}px`;
            this.imageElement.style.top = `${this.colorElement.offsetTop + (this.colorElement.offsetHeight / 2) - (this.imageElement.offsetHeight / 2)}px`
        }
    },
    methods: {

        updateImagePosition(e) {
            if (this.colorElement.offsetWidth == this.mainContainerElement.offsetWidth
                || this.mainContainerElement.offsetWidth < 400) {
                this.imageElement.style.left = `${(this.mainContainerElement.offsetWidth / 2) - (this.imageElement.offsetWidth / 2)}px`;
                this.imageElement.style.top = `${this.colorElement.offsetTop - (this.imageElement.offsetHeight / 2)}px`
            }
            else {
                this.imageElement.style.left = `${this.colorElement.offsetWidth - (this.imageElement.offsetWidth / 2)}px`;
                this.imageElement.style.top = `${this.colorElement.offsetTop + (this.colorElement.offsetHeight / 2) - (this.imageElement.offsetHeight / 2)}px`
            }
        }
    }
}
</script>

<style scoped>
.contact-container {
    height: 500px;
    max-height: 500px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.contact-color-container {
    height: 100%;
    min-width: 400px;
    flex-grow: 1;
}

.first-color {
    background-color: #024F78;
}

.second-color {
    background-color: #CAE7F7;
}

.contact-image {
    width: 300px;
    height: 444px;
    position: absolute;
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