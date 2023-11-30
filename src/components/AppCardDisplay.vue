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
<style></style>