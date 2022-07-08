<template>
        <section class="content">
            <div class="jumbo">
                <div class="box-text">CURRENT SERIES</div>
            </div>

            <div class="container">
                <div class="comic-list">
                    <ComicCard v-for="element, index in comics" :key="index" :cardSpecifics="element" />
                </div>
            </div>
        </section>
</template>

<script>
import ComicCard from './ComicCard.vue';
import ComicJson from '../assets/dc-comics.json';

export default {
    name: 'MainContent',
    components: {
        ComicCard
    },
    data() {
        return {
            comics: ComicJson
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    .content {
        background-color: #1c1c1c;
        color: $secondary_color;
        height: 900px;

        .jumbo {
            height: 300px;
            background-image: url('../assets/img/jumbotron.jpg');
            background-size: cover;
            position: relative;

            .box-text {
                color: $secondary_color;
                background-color: $primary_color;
                padding: 10px 15px;
                display: inline;
                position: absolute;
                bottom: -20px;
                left: 250px;
            }
        }
        .container {
            display: block;

            .comic-list {
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
            }
        }
    }
</style>