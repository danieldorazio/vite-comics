<script>
export default {
    props: {
        thumb: String,
        series: String,
    }
}
</script>

<template>
    <div>
        <img :src="thumb" alt="">
        <span>{{ series }}</span>
    </div>
</template>
<style lang="scss" scoped>
@use "../style/AppCardsComics.scss"
</style>