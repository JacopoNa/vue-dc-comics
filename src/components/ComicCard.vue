<template>
    <div class="single-card">
        <div class="image-card">
            <img :src="cardSpecifics.thumb" :alt="cardSpecifics.series">
        </div>

        <h4>{{ cardSpecifics.series }}</h4>
    </div>
</template>

<script>
export default {
    name: 'ComicCard',
     props: {
        cardSpecifics: Object
    }
}
</script>

<style lang="scss" scoped>
    .single-card {
        margin-top: 50px;
        width: calc((100% / 6) - 6px);

        .image-card {
            margin-bottom: 15px;
            height: 150px;
            width: 150px;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
    }
</style>