<template>
    <section class="main_container">
        <div class="first-part-container">
            <div class="first-part-text-container">
                <h2>TRATAMIENTO ORTOPÉDICO QUIRÚRGICO</h2>
                <p style="font-size: 17px;">En el ámbito de la cirugía ortopédica se realizan diferentes tipos de cirugías en pacientes, las
                    cuales son desarrolladas de la manera tradicional o bajo cirugía abierta o artroscópica. Las
                    cirugías más comunes incluyen:</p>
            </div>
            <div class="img"></div>
        </div>
        <div class="list-paragraph">
            <ul>
                <li><b>Artroscopía,</b> procedimiento que utiliza cámaras y equipos especiales para visualizar, diagnosticar y tratar problemas dentro de las articulaciones.</li>
                <li><b>Sutura de meniscos,</b> muy importante para preservar esta estructura fundamental para evitar la artrosis.</li>
                <li><b>Reemplazo parcial, total y revisión de las articulaciones,</b> proceso que se realiza cuando una articulación con artritis o dañada se retira y es reemplazada con una prótesis. Es una cirugía de alta complejidad.</li>
                <li><b>Osteotomía,</b> corrección de la deformación de un hueso sea cortándolo o reposicionando el hueso.</li>
                <li><b>Reparación del tejido,</b> reparación de un tejido, tal es el caso de tendones desgarrados o ligamentos.</li>
            </ul>

        </div>
    </section>
</template>

<script>
export default {
    name: "specialties"
}
</script>

<style scoped>
.main_container {
    padding: 50px 15%;
    background-color: #CAE7F7;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.first-part-container {
    display: flex;
    flex-wrap: wrap;
}

.first-part-text-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 60%;
    margin-right: 5%;
}

.title {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border: 1px solid red;
}

.list-paragraph {
    padding: 1rem 0;
    font-size: 17px;
}

.img {
    background: url('../assets/doctor_cirujano_extraño.jpg') no-repeat;
    height: 30vh;
    background-size: cover;
    background-position: center;
    border-radius: 1rem;
    width: 35%;
}

@media (max-width: 520px) {

    .img {
        width: 100%;
    }

    .first-part-text-container {
        width: 100%;
        margin-right: 0px;
    }
}
</style>