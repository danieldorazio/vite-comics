<script>
    export default {
        data () {
            return {
                mainList:[
                    
                    {
                        title: "DC COMICS",
                        link: [
                            "Characters",
                            "Comics",
                            "Movies",
                            "Tv",
                            "Games",
                            "Videos",
                            "News"
                        ],
                    },
                    
                    {
                        title: "DC",
                        link: [
                            "Terms Of Use",
                            "Privacy policy (New)",
                            "Ad Choices",
                            "Adventising",
                            "Jobs",
                            "Subscriptions",
                            "Talent Workshops",
                            "CPSC Certificates",
                            "Ratings",
                            "Shop Help",
                            "Contact Us"
                        ],
                    },
                    
                    {
                        title: "SITES",
                        link: [
                            "DC",
                            "MAD Magazine",
                            "DC Kids",
                            "DC Universe",
                            "DC Power Visa ",
                        ],
                    },
                    
                    {
                        title: "SHOP",
                        link: [
                            "Shop DC",
                            "Shop DC Collectibles",
                        ],
                    },


                ],   
            };
            
        },
    };

</script>

<template>
    <section >
        <section class="container">
            <div class="lists">
                <ul v-for="(list, index) in mainList">
                    <li class="title"><h2>{{ list.title }}</h2></li>
                    <li  v-for="(list, index) in list.link"><a class="link" href="">{{ list }}</a></li>
                </ul>
            </div>

            <img src="../assets/img/dc-logo-bg.png" alt="">
        </section>
    </section>
</template>

<style scoped lang="scss">
@use "../style/AppMainList.scss";
</style>