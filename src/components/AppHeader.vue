<template lang="">
    <header>
        <section class="container">
            <section class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC logo">
            </section>
            <nav class="navigation">
                <ul>
                    <li>
                        Characters
                    </li>
                    <li>
                        Comics
                    </li>
                    <li>
                        Movies
                    </li>
    
                </ul>
            </nav>
        </section>
    </header>
</template>
<script>
export default {
    name: "AppHeader",
}
</script>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

header {
    background-color: $header-bg-color;
    margin-top: 15px;
}

section.container {
    @include flex(row, space-between, center);
    width: 1100px;
    margin: 0 auto;
    padding: 1rem;
    font-size: .8rem;
    text-transform: uppercase;
}

section.logo > img {
    width: 70px;
}

nav.navigation > ul {
    @include flex(row, center, center);
    list-style: none;

    li {
        margin-right: 1rem;
    }
}

</style>