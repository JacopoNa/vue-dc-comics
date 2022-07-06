<template>
        <section class="content">
            <div class="container">
                <span> --> Content goes here </span>
            </div>
        </section>
</template>

<script>
export default {
    name: 'MainContent'
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    .content {
        background-color: #1c1c1c;
        color: $secondary_color;
        padding: 40px 0;
    }
</style>