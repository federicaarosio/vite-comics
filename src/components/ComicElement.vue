<template>
    <article>
        <h2>
            Comic Element
        </h2>
    </article>
</template>
<script>
export default {
    name: 'ComicElement',
}
</script>
<style lang="scss">
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    article {
        background-color: white;
        width: calc(100% / 6);
    }
</style>