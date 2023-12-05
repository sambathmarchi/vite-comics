<script>
import AppCard from './AppCard.vue'
export default {
    name: "AppContent",
    props: ["myseries"],
    components: {
        AppCard
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="seriesAbsolute">CURRENT SERIES</div>
            <AppCard v-for="elemento in myseries" :mycard="elemento"/>
            <button>LOAD MORE</button>
        </div>
    </section>
</template>

<style scoped>

section {
    background-color: #1C1C1C;
    color: white;
}
.container {
    width: 1100px;
    margin: 0 auto;
    padding: 30px 0;
    min-height: 130px;
    display: flex;
    flex-wrap: wrap;
    position: relative;
}

button {
    background-color: #0282F9;
    border: none;
    color: white;
    padding: 10px 40px;
    margin: 0 auto;
}

.seriesAbsolute {
    background-color: #0282F9;
    padding: 10px 40px;
    font-weight: 600;
    position: absolute;
    top: -20px;
    left: -10px;
    box-shadow: 4px 5px 2px 0px rgba(0,0,0,0.85);
}
</style>