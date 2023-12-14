<template lang="">
    <main>
           -- Content goes here --
    </main>
</template>
<script>
export default {
    name: "AppMain",
}
</script>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    
    main {
        width: 1100px;
        margin: 0 auto;
        padding: 2rem 0;
        color: $main-text-color;
        @include flex(row, start, center);

        font-size: .7rem;
    }
    
</style>