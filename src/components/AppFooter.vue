<script>
    export default {
        data () {
            return {
                social:
                {
                    title: "FOLLOW US",
                    socialLink:[
                        "img/footer-facebook.png",
                        "img/footer-twitter.png",
                        "img/footer-youtube.png",
                        "img/footer-pinterest.png",
                        "img/footer-periscope.png",
                    ],
                },
            };
        },

        methods: {
            getImagePath: function(img) {
                return new URL(`../assets/${img}`, import.meta.url).href;
            }
        },
    };
</script>

<template>
    <section>
        <div class="container">
            <button>SIGN-UP NOW</button>
        
            <div class="social">
                <ul>
                    <li class="title">{{ social.title }}</li>
                    <li class="icon" v-for="icon in social.socialLink"><img :src="getImagePath(icon)" alt=""></li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
    @use "../style/AppFooter.scss"
</style>