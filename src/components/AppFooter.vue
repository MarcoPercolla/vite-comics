<script>
export default {
    name: "AppFooter",
    data() {
        return {
            socialSrc: [
                "../../img/footer-facebook.png",
                "../../img/footer-periscope.png",
                "../../img/footer-twitter.png",
                "../../img/footer-pinterest.png",
                "../../img/footer-youtube.png"
            ]
        }
    },
    mounted() {
        console.log("Componente AppFooter caricato");
    }
}
</script>
<template>
    <div class="murales">
        <div class="footerLinks"></div>
        <div class="bgLogo">

        </div>
    </div>
</template>
<style scoped>
.murales {
    display: flex;
    padding: 0 10%;
    height: 20rem;
    background-image: url("../../img/footer-bg.jpg");
    background-size: cover;
}

.footerLinks {
    width: 60%;
}

.bgLogo {
    width: 40%;
    background-size: cover;
    background-position: center;
    background-image: url("../../img/dc-logo-bg.png");
}
</style>