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
    <ul v-for="(list, index) in mainList">
        <li><h2>{{ list.title }}</h2></li>
        <li v-for="(list, index) in list.link"><a href="">{{ list }}</a></li>
    </ul>
</template>

<style scoped>

</style>