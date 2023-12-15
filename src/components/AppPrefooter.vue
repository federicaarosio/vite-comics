<template>
    <section class="pre-footer">
        <div class="container">
            <div class="wrapper">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <p>Digital comics</p>
            </div>
            <div class="wrapper">
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                <p>DC merchandise</p>
            </div>
            <div class="wrapper">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                <p>Subscription</p>
            </div>
            <div class="wrapper">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <p>Comic shop locator</p>
            </div>
            <div class="wrapper">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                <p>DC power visa</p>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: "AppPrefooter",
}
</script>
<style lang="scss">
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

section.pre-footer {
    background-color: $accent;
    
    div.container {
        @include flex(row, center, center);
        width: 1100px;
        margin: 0 auto;
        padding: 3rem 0;
        color: $main-text-color;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: .8rem;
        text-transform: uppercase;
        gap: 2rem;
        
        div.wrapper {
            width: calc(100% / 5);
            @include flex(row, center, center);
            gap: .5rem;

            img {
                height: 50px;
            }
        }
    }

}
    
</style>