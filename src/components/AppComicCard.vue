<script>
export default {
    props: {
        comicId: Object
    }
}

</script>
<template>
    <div>
        <img :src="comicId.thumb" alt="">
    </div>
</template>
<style></style>