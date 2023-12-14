<template lang="">
    <header>
        <section class="container">
            <section class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC logo">
            </section>
            <nav class="navigation">
                <ul>
                    <li v-for="link in navLinks" :class="(link.active) ? 'active' : ''">
                        <!-- <a :href="link.url"> -->
                        {{link.content}}
                        <!-- </a> -->
                    </li>
                </ul>
            </nav>
        </section>
    </header>
</template>
<script>
export default {
    name: "AppHeader",
    data() {
        return {
            navLinks : [
                {
                    content: 'Characters',
                    url: '#',
                    active: false,
                },

                {
                    content: 'Comics',
                    url: '#',
                    active: true,
                },

                {
                    content: 'Movies',
                    url: '#',
                    active: false,
                },

                {
                    content: 'TV',
                    url: '#',
                    active: false,
                },

                {
                    content: 'Games',
                    url: '#',
                    active: false,
                },
                
                {
                    content: 'Collectibles',
                    url: '#',
                    active: false,
                },
                
                {
                    content: 'Videos',
                    url: '#',
                    active: false,
                },
                
                {
                    content: 'Fans',
                    url: '#',
                    active: false,
                },
                
                {
                    content: 'News',
                    url: '#',
                    active: false,
                },
                
                {
                    content: 'Shop',
                    url: '#',
                    active: false,
                },
            ],
        }
    },
}
</script>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

header {
    background-color: $header-bg-color;
    margin-top: 15px;

    section.container {
        @include flex(row, space-between, center);
        width: 1100px;
        margin: 0 auto;
        padding: 1rem;
        font-size: .8rem;
        text-transform: uppercase;
    }

}


section.logo > img {
    width: 70px;
}

nav.navigation > ul {
    @include flex(row, center, center);
    list-style: none;

    li {
        margin-right: 1rem;
        &.active {
            color: $accent;
            border-bottom: 3px solid $accent;
        }
    }
}

</style>