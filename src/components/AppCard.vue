<script>
export default {
    name: "AppCard",
    props: {
        mycard: Object,
    }
}

</script>





<template>
    <div class="card">
        <img class="imgMb" :src="mycard.thumb" alt="">
        <p class="pMb">{{ mycard.series.toUpperCase() }}</p>
    </div>
</template>






<style scoped>
.card {
    padding: 5px;
    width: calc(100% / 6 - 10px);
}

img {
    width: 100%;
    height: 150px;
    object-fit: cover;
    object-position: top;
}

.imgMb {
    margin-bottom: 10px;
}

.pMb {
    margin-bottom: 20px;
}

</style>