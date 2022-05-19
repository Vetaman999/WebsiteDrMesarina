<template>
    <div class="my-5 ml-5" style="width: 90%; display: flex; justify-content: space-between; align-items: center;">
        <h2 style="font-size:35px; color:#2397D7;">{{separate}}</h2>
        <hr style="width: 70%; height: 2px; background-color: #6789a1; border: #6789a1;"/>
    </div>
</template>

<script>
export default {
    name: 'call-to-reserve',
    props: {
        separate: String
    }
}
</script>