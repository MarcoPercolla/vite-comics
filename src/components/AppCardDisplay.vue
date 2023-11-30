<script>
import AppComicCard from './AppComicCard.vue'

export default {

    props: ["catalog"],
    components: {
        AppComicCard
    }
}
</script>
<template>
    <section class="dcCards">
        <div class="fakeBtn">
            <h2>CURRENT SERIES</h2>
        </div>
        <div class="cardsContainer">
            <AppComicCard v-for="comic in catalog" :comicId="comic" />

        </div>
        <div class="fakeBtn2">
            <h2>LOAD MORE</h2>
        </div>
    </section>
</template>
<style scoped>
.cardsContainer {

    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 0.5rem 10%;
}

.dcCards {
    background-color: #222;
    position: relative;
    padding: 2rem 0;

}

.fakeBtn {
    width: 12rem;
    height: 2.5rem;
    font-size: 0.8rem;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: rgb(0, 110, 255);
    position: absolute;
    top: -1rem;
    left: 10%
}

.fakeBtn2 {
    width: 10rem;
    height: 2.5rem;
    font-size: 0.6rem;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: rgb(0, 110, 255);
    margin: 0.5rem auto;
}
</style>