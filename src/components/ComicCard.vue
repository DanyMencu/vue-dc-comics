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

    .img-container {
        width: 100%;
        height: 60%;
        overflow: hidden;

        img {
            width: 100%;
        }
    }

    a {
        text-decoration: none;

        h4 {
            color: #fff;
            padding: 1rem 0;
            text-transform: uppercase;
        }
    }
</style>