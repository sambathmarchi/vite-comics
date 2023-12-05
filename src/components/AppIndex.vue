<script>

export default {
    name: "AppIndex",
    data () {
        return {
            index: [
                {
                    title: "DC COMIC",
                    i: [ "Characters", "Comics", "Movies", "TV", "Games", "Videos", "News", ]
                },
                {
                    title: "SHOP",
                    i: [ "Shop DC", "Shop DC Collectribles"]
                },
                {
                    title: "DC",
                    i: [ "Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subsctiptions", "Talent Workshops", "CPSC Cerificates", "Ratings", "Shop Help", "Contact Us" ]
                },
                {
                    title: "SITES",
                    i: [ "DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
                <div class="sfondo">
                    <div class="marginIndex">
                        <div class="spaceTitle" v-for="element in index">
                            <h3>{{element.title}}</h3>
                            <p v-for="item in element.i">{{ item }}</p>
                        </div>
                    </div>
                </div>
        </div>
    </section>
</template>

<style scoped>

section {
    background-image: url(/img/footer-bg.jpg);
    width: 100%;
    background-repeat: no-repeat;
    background-size: cover;
    color: white;
}

img {
    display: block;
}

.container {
    width: 1100px;
    margin: 0 auto;
    min-height: 130px;
}

.sfondo {
    background-image: url(/img/dc-logo-bg.png);
    min-height: 340px;
    background-repeat: no-repeat;
    background-position: right;
}

.marginIndex {
    padding: 30px 0;
    height: 340px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    width: 40%;
}

h3 {
    margin-bottom: 1rem;
}

p {
    font-size: 12px;
    color: #949494;
    margin-bottom: 0.3rem;
}

.spaceTitle {
    margin-bottom: 1rem;
}

</style>
