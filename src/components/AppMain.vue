<template lang="">
    <main>
           <section class="jumbo"></section>
           <section class="comics">Comics</section>
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
        section.jumbo {
            background-image: url(../assets/img/jumbotron.jpg);
            background-size: cover;
            height: 20rem;
        }
    }
    
</style>