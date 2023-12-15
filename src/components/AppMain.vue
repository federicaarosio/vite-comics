<template lang="">
    <main>
           <section class="jumbo">
        </section>
        <section class="comics">
            <ComicElement v-for="comic in comicsList"
            :thumb="comic.thumb"
            :price="comic.price"
            :series="comic.series"
            :type="comic.type"
            />
            <p>Current Series</p>
        </section>
        <div>
            <button>
                load more
            </button>
        </div>
        <AppPrefooter />
    </main>
</template>
<script>
import ComicElement from './ComicElement.vue';
import AppPrefooter from './AppPrefooter.vue';

export default {
    name: "AppMain",
    data() {
        return {
            comicsList: [
                            {
                                "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                                "price": "$19.99",
                                "series": "Action Comics",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                                "price": "$3.99",
                                "series": "American Vampire 1976",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                                "price": "$16.99",
                                "series": "Aquaman",
                                "type": "graphic novel",
                            },
                            {
                                "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                                "price": "$2.99",
                                "series": "Batgirl",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                                "price": "$3.99",
                                "series": "Batman",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                                "price": "$2.99",
                                "series": "Batman Beyond",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                                "price": "$3.99",
                                "series": "Batman/Superman",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                                "price": "$4.99",
                                "series": "Batman/Superman Annual",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                                "price": "$5.99",
                                "series": "Batman: The Joker War Zone",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                                "price": "$6.99",
                                "series": "Batman: Three Jokers",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                                "price": "$4.99",
                                "series": "Batman: White Knight Presents: Harley Quinn",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                                "price": "$16.99",
                                "series": "Catwoman",
                                "type": "graphic novel",
                            },
                ],
        }
    },
    components: {
        ComicElement,
        AppPrefooter
    }
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

        section.comics {
            width: 1100px;
            margin: 0 auto;
            @include flex(row, center, stretch);
            flex-wrap: wrap;
            gap: 1rem;
            padding-top: 4rem;
            margin-bottom: 3rem;
            position: relative;

            p {
                position: absolute;
                z-index: 0;
                left: 0;
                top: 0;
                transform: translate(0%, -50%); background-color: $accent;
                color: $main-text-color;
                padding: .5rem 1rem;
                text-transform: uppercase;
            }

        }

        div {
            text-align: center;
            margin-bottom: 3rem;
            
            button {
                text-align: center;
                background-color: $accent;
                color: $main-text-color;
                padding: .5rem 3rem;
                text-transform: uppercase;
                font-size: .9rem;
                font-weight: bold;
            }
        }

    }
    
</style>