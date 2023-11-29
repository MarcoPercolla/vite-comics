<script>

export default {
    name: "AppHeader",
    data() {
        return {
            products: [
                {
                    category: "DIGITAL COMIC",
                    src: "../../img/buy-comics-digital-comics.png",
                },
                {
                    category: "DC MERCHANDISE",
                    src: "../../img/buy-comics-merchandise.png",
                },
                {
                    category: "SUBSCRIPTION",
                    src: "../../img/buy-comics-shop-locator.png",
                },
                {
                    category: "COMIC SHOP LOCATOR",
                    src: "../../img/buy-comics-subscriptions.png",
                },
                {
                    category: "DC POWER VISA",
                    src: "../../img/buy-dc-power-visa.svg",
                },
            ]
        }
    },
    mounted() {
        console.log("Componente AppHeader caricato");
    }
}
</script>
<template>
    <div class="vetrina">
        <div class="card" v-for="product in products">
            <img :src="product.src" alt="">
            <h4>{{ product.category }}</h4>

        </div>

    </div>
</template>
<style scoped>
.vetrina {
    height: 8rem;
    background-color: rgb(0, 123, 255);
    display: flex;
    padding: 1rem 10%;
    align-items: center;
    justify-content: space-around;
    color: white;
}

.card {
    width: 20%;
    display: flex;
    align-items: center;

}

img {
    max-height: 3rem;
    max-width: 3rem;
    margin-right: 1rem;
}
</style>