<template>
    <article>
         <img :src="thumb" :alt="series">

        <p>
            {{series}}
        </p>
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
        color: $main-text-color;
        width: calc((100% / 6) - 2rem);
        margin-bottom: 1rem;

        img {
            width: 100%;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: top;
            margin-bottom: 1rem;
        }

        p {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: .8rem;
            text-transform: uppercase;
        }
    }
</style>