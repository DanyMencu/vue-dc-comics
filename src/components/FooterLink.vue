<template>
  <section>
        <div class="container d-flex s-between footer-links">
            <!-- Links -->
            <div class=" d-flex py-1_5">
                <div>
                    <h3>Dc Comics</h3>
                    <ul>
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
                            <a href="/">TV</a>
                        </li>
                        <li>
                            <a href="/">Games</a>
                        </li>
                        <li>
                            <a href="/">Videos</a>
                        </li>
                        <li>
                            <a href="/">News</a>
                        </li>
                    </ul>
                    <h3>Shop</h3>
                    <ul>
                        <li>
                            <a href="/">Shop DC</a>
                        </li>
                        <li>
                            <a href="/">Shop DC Collectibles</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3>Dc</h3>
                    <ul>
                        <li>
                            <a href="/">Therms Of Use</a>
                        </li>
                        <li>
                            <a href="/">Privacy policy (New)</a>
                        </li>
                        <li>
                            <a href="/">Ad Choices</a>
                        </li>
                        <li>
                            <a href="/">Advertising</a>
                        </li>
                        <li>
                            <a href="/">Jobs</a>
                        </li>
                        <li>
                            <a href="/">Subscriptions</a>
                        </li>
                        <li>
                            <a href="/">Talent Workshops</a>
                        </li>
                        <li>
                            <a href="/">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="/">Rating</a>
                        </li>
                        <li>
                            <a href="/">Shop Help</a>
                        </li>
                        <li>
                            <a href="/">Contact Us</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3>Sites</h3>
                    <ul>
                        <li>
                            <a href="/">DC</a>
                        </li>
                        <li>
                            <a href="/">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="/">DC Kids</a>
                        </li>
                        <li>
                            <a href="/">DC Universe</a>
                        </li>
                        <li>
                            <a href="/">DC Power Visa</a>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- Big logo -->
            <img src="@/assets/dc-logo-bg.png" alt="DC logo big">
        </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped lang='scss'>
    section {
        height: 45vh;
        background-image: url('../assets/footer-bg.jpg');
        color: #fff;

        img {
            object-fit: cover;
            width: 400px;
        }

            h3 {
                margin: 5px 0 7px;
                font-size: 13px;
                text-transform: uppercase;
            }

        ul {
            list-style: none;

            li {
                line-height: 13px;
                margin-right: 30px;
            }

            li:last-child {
                margin-bottom: 20px;
            }

             a {
                text-decoration: none;
                color: #fff;
                font-size: 10px;
            }

        }
    }
</style>