<script>
export default {
    props: {
        thumb: String,
        series: String,
    }
}
</script>

<template>
    <div class="card">
        <img :src="thumb" alt="">
        <a href="">{{ series }}</a>
    </div>
</template>
<style lang="scss" scoped>
@use "../style/AppCardsComics.scss"
</style>