<template>
    <div class="calltoreserve-container">
        <div class="container-text">
            <div>
                <h2 class="calltoreserve-title">Llámanos para reservar tu consulta</h2>
                <p class="calltoreserve-text">Si tienes y quieres una consulta... Llámanos con toda confianza. Nosotros lo vamos a ayudar</p>
            </div>
        </div>
        <div class="container-btn">
            <v-btn style="padding: 25px 12px; font-weight: 700;" color="#80CCF6">Llámanos +51 947 358 498</v-btn>
        </div>
    </div>
</template>

<style scoped>

.calltoreserve-container {
    display: flex;
    width: 100%;
    background-color: #287DAA;
}

.container-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex: 3;
    margin: 40px 0;
}

.calltoreserve-title {
    color: white;
    margin: 10px 0 10px 0;
    font-size: 40px;
}

.calltoreserve-text {
    color: white;
    margin: 10px 0 10px 0;
    font-weight: lighter;
}

.container-btn {
    display: flex;
    justify-content: center;
    align-items: center;
    flex: 2;
}

</style>