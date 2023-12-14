<template lang="">
    <footer>
        <section class="upper-footer">
            <section class="navigation">
                <section class="first-col">
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
                </section>
                <section class="second-col">
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
                </section>
                <section class="third-col">
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
                </section>
            </section>
            <section class="footer-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </section>
        </section>
        <section class="signup-socials"></section>
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

        section.footer-logo > img {
            width: 400px;
            overflow: hidden;
        }
    }
}
    
</style>