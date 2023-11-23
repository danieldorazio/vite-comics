<script>
    export default {
        data () {
            return {
                navBar: [
                    
                    {
                        text: "CHARACTERS",
                    },

                    {
                        text: "COMICS",
                    },

                    {
                        text: "MOVIES",
                    },

                    {
                        text: "TV",
                    },

                    {
                        text: "GAMES",
                    },

                    {
                        text: "COLLECTIBLES",
                    },

                    {
                        text: "VIDEOS",
                    },

                    {
                        text: "FANS",
                    },

                    {
                        text: "NEWS",
                    },

                    {
                        text: "SHOP",
                    },
                ]
            };
        },
    };
</script>

<template>
    <header class="container p-top-bottom">
        <img src="../assets/img/dc-logo.png" alt="">

        <ul>
            <li v-for ="navBarObj in navBar" ><a href="">{{ navBarObj.text }}</a></li>
        </ul>
    </header>
</template>

<style scoped lang="scss">
@use "../style/AppHeader.scss";
</style>