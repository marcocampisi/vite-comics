<script>
export default {
    name: "Comic",
    data() {
        return {

        }
    },
    props: {
        comicThumb: String,
        comicPrice: String,
        comicSeries: String,
        comicType: String
    }
}
</script>

<template>
    <div class="comic">
        <div class="thumbContainer">
            <img :src="comicThumb" :alt="comicSeries">
        </div>
        <h3>{{ comicSeries }}</h3>
    </div>
</template>

<style lang="scss" scoped>

</style>