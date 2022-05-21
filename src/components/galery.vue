<template>
<div>
    <div style="margin-top:10px">
        <v-card-title class="justify-center pb-5" style="margin-bottom: 10px;font-size: 3vw ; color: #024F78;">
            GALERY
        </v-card-title>
        <hr width="40%" class="mx-auto" style="border:1px solid #024F78">
    </div>
    <div class="container-img">
        <div class="box-img">
            <a>
                <figure>
                    <img src="../assets/IMG_1780.png">
                </figure>
            </a>
        </div>
        <div class="box-img">
            <a>
                <figure>
                    <img src="../assets/IMG_1771.png">
                </figure>
            </a>
        </div>
        <div class="box-img">
            <a>
                <figure>
                    <img src="../assets/IMG_1774.png">
                </figure>
            </a>
        </div>
        <div class="box-img">
            <a>
                <figure>
                    <img src="../assets/ope.png">
                </figure>
            </a>
        </div>
        <div class="box-img">
            <a>
                <figure>
                    <img src="../assets/IMG_1782.png">
                </figure>
            </a>
        </div>
        <div class="box-img">
            <a>
                <figure>
                    <img src="../assets/IMG_1775.png">
                </figure>
            </a>
        </div>
        <div class="box-img">
            <a>
                <figure>
                    <img src="../assets/IMG_1784.png">
                </figure>
            </a>
        </div>
    </div>
</div>
</template>

<script>    
</script>

<style scoped>
.container-img{
    width: 100%;
    max-width: 1100px;
    margin: auto;
    margin-top: 60px;
    margin-bottom: 60px;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: 250px;
    grid-gap: 20px;
}
.container-img .box-img figure{
    width: 100%;
    height: 100%;
}
.container-img .box-img img{
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.container-img .box-img:nth-child(1){
    grid-column-start:span 2;
}
.container-img .box-img:nth-child(4){
    grid-column-start:span 2;
}

</style>