<template>
  <section>
      <div class="container d-flex s-between">
            <a href="/">
                <img  class="header-logo" src="@/assets/dc-logo.png" alt="DC logo">
            </a>
            <ul class="d-flex i-center">
                <li>
                    <a href="/">Characters</a>
                </li>
                <li>
                    <a href="/">Comics</a>
                </li>
                <li>
                    <a href="/">Movies</a>
                </li>
                <li>
                    <a href="/">Tv</a>
                </li>
                <li>
                    <a href="/">Games</a>
                </li>
                <li>
                    <a href="/">Collectibles</a>
                </li>
                <li>
                    <a href="/">Videos</a>
                </li>
                <li>
                    <a href="/">Fans</a>
                </li>
                <li>
                    <a href="/">News</a>
                </li>
                <li>
                    <a href="/">Shop</a>
                </li>
            </ul>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped lang='scss'>
    
    section {
        height: 10vh;
        margin: 15px 0;
    }

    .container > a {
        height: 100%;
    }

        .header-logo {
        height: 100%;
        padding: 0.25rem;
        transition: filter 0.2s;

        &:hover {
            filter:grayscale(0.5);
        }
    }

    ul {
        height: 100%;
        justify-content: center;
        list-style: none;

        li {
            position: relative;
            margin: 0 0.6rem;

            a {
                display: inline-block;
                text-decoration: none;
                color: #000;
                text-transform: uppercase;
                font-size: 12px;
                font-weight: 600;
            }
        }

        li::after {
            content: "";
            display: inline-block;
            position: relative;
            top: 28px;
            width: 100%;
            height: 0;
            background: #0b5ba5;
            transition: height 0.15s;
        }

        li:hover::after {
            height: 2px;
        }

        li:hover a {
            color: #0b5ba5;
        }
    }

</style>