<script>
export default {
    name: "AppLinks",
    data () {
        return {
            links: [
                {
                    img: "/img/buy-comics-digital-comics.png",
                    nome: "DIGITAL COMICS"
                },
                {
                    img: "/img/buy-comics-merchandise.png",
                    nome: "DC MERCHANDISE"
                },
                {
                    img: "/img/buy-comics-subscriptions.png",
                    nome: "SUBSCRIPTION"
                },
                {
                    img: "/img/buy-comics-shop-locator.png",
                    nome: "COMIC SHOP LOCATOR"
                },
                {
                    img: "/img/buy-dc-power-visa.svg",
                    nome: "DC POWER VISA"
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="elementLink" v-for="element in links">
                <img :src="element.img" :alt="element.nome">
                <a href="#">{{ element.nome }}</a>
            </div>
        </div>
    </section>
</template>

<style scoped>

section {
    background-color: #0282F9;
    color: white;
}
.container {
    width: 1100px;
    margin: 0 auto;
    min-height: 130px;
    display: flex;
    align-items: center;
}

img {
    margin-right: 1rem;
    height: 50px;
}

.elementLink {
    align-items: center;
    display: flex;
    justify-content: center;
    width: 100%;
}

a {
    font-size: 12px;
    text-decoration: none;
    color: white;
}
</style>










