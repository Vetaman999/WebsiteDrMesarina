<template>
    <div class="calltoreserve-container">
        <div class="container-empty"></div>
        <div class="container-text">
            <div>
                <h2 class="calltoreserve-title">{{title}}</h2>
                <p class="calltoreserve-text">{{subTitle}}</p>
            </div>
        </div>
        <div class="container-btn">
            <v-btn style="background-color: #2397D7; color: white; height: 61px; width: 310px;">
                <v-card-text style="font-size:20px; font-weight: lighter; color:#FFFFFF">
                    {{btnText}}
                </v-card-text>
            </v-btn>
        </div>
        <div class="container-empty"></div>
    </div>
</template>

<script>
export default {
    name: 'call-to-reserve',
    props: {
        title: String,
        subTitle: String,
        btnText: String
    }
}
</script>

<style scoped>
.calltoreserve-container {
    display: flex;
    width: 100%;
    background-color: #287DAA;
    flex-wrap: wrap;
    padding: 70px 0;
}

.container-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex: 9;
}

.calltoreserve-title {
    color: white;
    margin: 10px 0 10px 0;
    font-size: 45px;
}

.calltoreserve-text {
    color: white;
    padding: 0px 10px 0px 0;
    font-weight: lighter;
    font-size: 20px;
}

.container-btn {
    display: flex;
    justify-content: center;
    align-items: center;
    flex: 4;
}

.container-empty {
    flex: 1;
}
</style>