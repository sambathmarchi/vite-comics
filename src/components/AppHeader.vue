<script>
export default {
    name: "AppHeader",
    data() {
        return {
            navbar: [
                "CHARACTER", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"
            ]
        }
    }
}
</script>

<template>
    <section>
        <nav class="container">
            <div>
                <img src="/img/dc-logo.png" alt="logo">
            </div>
            <div>
                <a class="border" href="#" v-for="element in navbar">{{ element }}</a>
            </div>
        </nav>
    </section>
</template>

<style scoped>
section {
    background-color: white;
}

img {
    display: block;
}

.container {
    width: 1100px;
    margin: 0 auto;
    min-height: 130px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

a {
    margin-left: 1rem;
    font-weight: 600;
    text-decoration: none;
    color: black;
    height: 130px;
    display: inline-block;
    line-height: 130px;
}

a:hover{
    color: #0282F9;
    border-bottom: 5px solid #0282F9;
}
</style>
