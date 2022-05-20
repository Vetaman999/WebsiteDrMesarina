<template>
    <v-card class="mx-auto" elevation="0" color="transparent">
        <div class="convention-title">
            Nuestros Convenios
        </div>
        <hr width="70%" class="mx-auto" style="border:1px solid #024F78">
        <v-container class="px-5" style="border-color: #024F78;">
            <v-container grid-list-md>
                <v-layout row wrap>
                    <v-card class="mx-auto" width="200px" elevation="0" color="transparent">
                        <v-img class="mx-auto" src="../assets/espon1.jpg" width="150px" height="100px"></v-img>
                    </v-card>
                    <v-card class="mx-auto" width="200px" elevation="0" color="transparent">
                        <v-img class="mx-auto" src="../assets/espon2.jpg" width="150px" height="100px"></v-img>
                    </v-card>
                    <v-card class="mx-auto" width="200px" elevation="0" color="transparent">
                        <v-img class="mx-auto" src="../assets/spon3.jpg" width="150px" height="100px"></v-img>
                    </v-card>
                    <v-card class="mx-auto" width="200px" elevation="0" color="transparent">
                        <v-img class="mx-auto" src="../assets/espon4.jpg" width="150px" height="100px"></v-img>
                    </v-card>
                    <v-card class="mx-auto" width="200px" elevation="0" color="transparent">
                        <v-img class="mx-auto" src="../assets/espon5.jpg" width="150px" height="100px"></v-img>
                    </v-card>
                </v-layout>
            </v-container>
        </v-container>
    </v-card>
</template>

<style>
.convention-title {
    padding-bottom: 5px;
    font-size: 4vw;
    font-weight: 500;
    text-align: center;
    color: #024F78;
}


@media (max-width: 1000px) {
    .convention-title {
        font-size: 7vw;
    }
}
</style>