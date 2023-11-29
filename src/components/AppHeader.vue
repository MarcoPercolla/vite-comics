<script>
export default {
    name: "AppHeader",
    data() {
        return {
            menuLinks: [
                {
                    text: "Characters",
                    url: "#characters",
                },
                {
                    text: "Comics",
                    url: "#Comics",
                },
                {
                    text: "Movies",
                    url: "#Movies",
                },
                {
                    text: "Tv",
                    url: "#Tv",
                },
                {
                    text: "Games",
                    url: "#Games",
                },
                {
                    text: "Collectibles",
                    url: "#Collectibles",
                },
                {
                    text: "Videos",
                    url: "#Videos",
                },
                {
                    text: "Fans",
                    url: "#Fans",
                },
                {
                    text: "News",
                    url: "#News",
                },
                {
                    text: "Shop",
                    url: "#Shop",
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
    <header>
        <div class="imgContainer">
            <img id="logo" src="../../img/dc-logo.png" alt="">
        </div>
        <div id="linkChain">
            <a v-for="link in menuLinks" :href="link.url"> {{ link.text }}</a>
        </div>
    </header>
</template>
<style scoped>
header {
    padding: 1rem 10%;
    display: flex;
    align-items: center;
}

.imgContainer {
    width: 40%;
}

.linkChain {
    width: 60%;
}

a {
    margin: 1rem;
    text-decoration: none;
    color: black;
}

a:hover {
    color: rgb(0, 76, 255)
}
</style>