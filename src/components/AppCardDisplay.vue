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
    <div class="cardsContainer">
        <AppComicCard v-for="comic in catalog" :comicId="comic" />

    </div>
</template>
<style scoped>
.cardsContainer {
    background-color: #222;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 4rem 10%;
}
</style>