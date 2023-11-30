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
        <div class="footerLinks">
            <ul>
                <h5>DC COMICS</h5>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
                <ul>
                    <h5>SHOP</h5>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
            </ul>
            <ul>
                <h5>DC</h5>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Privacy policy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
            <ul>
                <h5>SITES</h5>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
            </ul>
        </div>

        <div class="bgLogo"> </div>
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

.footerLinks {

    display: flex;
    margin: 2rem;
}

h5 {
    margin: 0.8rem 0;
    color: white;
}

ul {
    margin: 0 0.5rem;
}

li {
    list-style: none;
    margin: 0.2rem;

}

a {
    color: grey;
    font-size: 0.7rem;
}
</style>