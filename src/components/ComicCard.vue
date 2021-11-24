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
        overflow: hidden;
        aspect-ratio: 1 / 1.3;

        img {
            transition: all 0.25s;
        }
    }

    a {
        text-decoration: none;


        &:hover img {
            filter:contrast(120%);
        }

         &:hover h4 {
             color: #198ffd;
            text-decoration: underline;
        }

        h4 {
            color: #fff;
            padding: 1rem 0;
            text-transform: uppercase;
            transition: color 0.25s;
        }
    }
</style>