<script>

export default {
    name: "AppSignFollow",
    data () {
        return {
            img: [
                "/img/footer-facebook.png",
                "/img/footer-twitter.png",
                "/img/footer-youtube.png",
                "/img/footer-pinterest.png",
                "/img/footer-periscope.png",
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div>
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="flexImg">
                <p class="marginFlexImg">FOLLOW US</p>
                <img class="marginFlexImg" v-for="element in img" :src="element" alt="">
            </div>
        </div>
    </section>
</template>

<style scoped>

section {
    background-color: #303030;
    color: #0282F9;
}

.container {
    width: 1100px;
    margin: 0 auto;
    min-height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

button {
    background-color: #303030;
    border: 2px solid #0282F9;
    padding: 1rem;
    color: white;
    font-weight: 600;
    cursor: pointer;
}

p {
    font-size: 20px;
    font-weight: 600;
}

.flexImg {
    display: flex;
    align-items: center;
}

.marginFlexImg {
    margin-left: 1rem;
}


</style>