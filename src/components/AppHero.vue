<script>

    export default {
        data () {
            return {
                heroImg: [
                    
                    {
                        img: "img/buy-comics-digital-comics.png",
                        text: "DIGITAL COMICS"
                    },

                    {
                        img: "img/buy-comics-merchandise.png",
                        text: "DC MERCHANDISE"
                    },

                    {
                        img: "img/buy-comics-subscriptions.png",
                        text: "SUBCRIPTION"
                    },

                    {
                        img: "img/buy-comics-shop-locator.png",
                        text: "COMIC SHOP LOCATOR"
                    },

                    {
                        img: "img/buy-dc-power-visa.svg",
                        text: "DC POWER VISA"
                    },
                ],
            };
        },

        methods: {
            getImagePath: function(img) {
                return new URL(`../assets/${img}`, import.meta.url).href;
            }
        }
    }
</script>

<template>
    <section>
        <div class="container">
            <ul v-for="element in heroImg">
                <li class="img"><img :src="getImagePath(element.img)" alt=""></li>
                <li class="text"><a href="">{{ element.text }}</a></li>
            </ul>
        </div>
    </section>
</template>

<style scoped lang="scss">
    @use "../style/AppHero.scss"
</style>