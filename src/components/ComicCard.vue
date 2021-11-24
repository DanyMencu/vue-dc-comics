<template>
    <a href="/">
        <div class="img-container">
            <img :src="thumb" :alt="series">
        </div>
        <h4> {{ series }} </h4>
    </a>
</template>

<script>
export default {
    name: 'ComicCard',
    props: {
        thumb: String,
        series: String,
    },

}
</script>

<style scoped lang='scss'>
        
</style>