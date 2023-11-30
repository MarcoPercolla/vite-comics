<script>
export default {
    props: {
        comicId: Object
    }
}

</script>

<template>
    <div class="card">
        <img :src="comicId.thumb" alt="">
        <h3>{{ comicId.series.toUpperCase() }}</h3>
    </div>
</template>

<style scoped>
.card {
    width: 13%;
    color: white;
    margin: 1rem;

}

img {
    width: 100%;
    aspect-ratio: 1 / 1;
    object-fit: cover;
    border-radius: 0.1rem;
}

h3 {
    font-size: 0.8rem;
}
</style>