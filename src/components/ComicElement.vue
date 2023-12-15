<template>
    <article>
        <img :src="thumb" alt="comic cover">
        <h2>
            {{series}}
        </h2>
    </article>
</template>
<script>
export default {
    name: 'ComicElement',
    props: {
        thumb: String,
        price : [Number, String],
        series: String,
        type: String,
    }
}
</script>
<style lang="scss">
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    article {
        background-color: white;
        width: calc(100% / 6);

        img {
            width: 100%;
        }
    }
</style>