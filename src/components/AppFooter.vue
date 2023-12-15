<template lang="">
    <footer>
        <section class="upper-footer">
            <section class="navigation">
                <div class="first-col">
                    <h1>
                        DC Comics
                    </h1>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h1>
                        Shop
                    </h1>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="second-col">
                    <h1>
                        DC
                    </h1>
                    <ul>
                        <li>Terms of Use</li>
                        <li>Privacy policy(New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="third-col">
                    <h1>
                        Sites
                    </h1>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>Ad Choices</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </section>
            <section class="footer-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </section>
        </section>
        <section class="lower-footer">
            <div class="wrapper">
                <button class="sign-up">
                    sign-up now!
                </button>
                <div class="socials">
                    <div class="follow-us">
                        Follow us
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-facebook-f"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-twitter"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-youtube"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-pinterest-p"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-solid fa-location-dot"></i>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: "AppFooter",
}
</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

footer {
    background-image: url(../assets/img/footer-bg.jpg);

    section.upper-footer {
        @include flex(row, space-between, center);
        height: 100%;
        width: 1100px;
        margin: 0 auto;

        section.navigation {
            @include flex(row, start, start);

            h1 {
                color: $main-text-color;
                text-transform: uppercase;
                margin: 1rem 0;
            }

            ul {
                margin-right: 2rem;

                li {
                    font-size: .7rem;
                    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
                    color: $small-text-color;
                    margin-bottom: .7rem;
                }
            }
        }

        section.footer-logo {
            height: 100%;

            img {
                overflow: hidden;
                width: 400px;
            }
        }
    }

    section.lower-footer {
        background-color: $footer-bg-color;

        div.wrapper {
            width: 1100px;
            margin: 0 auto;
            padding: 2rem 0;
            @include flex(row, space-between, center);

            button.sign-up {
                background-color: transparent;
                border: 2px solid $accent;
                color: $main-text-color;
                font-size: .8rem;
                font-weight: bold;
                padding: .8rem 1.2rem;
                text-transform: uppercase;

            }

            div.socials {
                @include flex(row, end, center);
                div.follow-us {
                    color: $accent;
                    font-size: 1rem;
                    font-weight: bold;
                    text-transform: uppercase;
                    margin-right: 1rem;

                }

                div.icon {
                    margin-right: 1rem;
                    color: $footer-bg-color;
                    background-color: $small-text-color;
                    width: 25px;
                    height: 25px;
                    border-radius: 50%;
                    @include flex(row, center, center)
                }
            }

        }
    }
}
    
</style>