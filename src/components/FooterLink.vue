<template>
  <section>
        <div class="container d-flex s-between footer-links">
            <!-- Links -->
            <div class=" d-flex py-1_5">
                <div>
                    <h3>Dc Comics</h3>
                    <ul>
                        <li v-for="(element, index) in Comics" :key="`comicIndex-${index}`">
                            <a :href="element.url">{{ element.text }}</a>
                        </li>

                    </ul>
                    <h3>Shop</h3>
                    <ul>
                        <li v-for="(element, index) in Shop" :key="`shopIndex-${index}`">
                            <a :href="element.url">{{ element.text }}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3>Dc</h3>
                    <ul>
                        <li v-for="(element, index) in Dc" :key="`DcIndex-${index}`">
                            <a :href="element.url">{{ element.text }}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3>Sites</h3>
                    <ul>
                        <li v-for="(element, index) in Sites" :key="`siteIndex-${index}`">
                            <a :href="element.url">{{ element.text }}</a>
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
    name:'FooterLinks',
    data() {
        return {
            Comics: [
                {
                    text: 'Characters',
                    url: '/'
                },
                {
                    text: 'Comics',
                    url: '/'
                },
                {
                    text: 'Movies',
                    url: '/'
                },
                {
                    text: 'TV',
                    url: '/'
                },
                {
                    text: 'Games',
                    url: '/'
                },
                {
                    text: 'Videos',
                    url: '/'
                },
                {
                    text: 'News',
                    url: '/'
                },
            ],
            Shop: [
                {
                    text: 'Shop DC',
                    url: '/',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '/',
                },
            ],
            Dc: [
                {
                    text: 'Therms Of Use',
                    url: '/',
                },
                {
                    text: 'Privacy policy (New)',
                    url: '/',
                },
                {
                    text: 'Ad Choices',
                    url: '/',
                },
                {
                    text: 'Advertising',
                    url: '/',
                },
                {
                    text: 'Jobs',
                    url: '/',
                },
                {
                    text: 'Subscriptions',
                    url: '/',
                },
                {
                    text: 'Talent Workshops',
                    url: '/',
                },
                {
                    text: 'CPSC Certificates',
                    url: '/',
                },
                {
                    text: 'Rating',
                    url: '/',
                },
                {
                    text: 'Shop Help',
                    url: '/',
                },
                {
                    text: 'Contact Us',
                    url: '/',
                },
            ],
            Sites: [
                {
                    text: 'DC',
                    url: '/',
                },
                {
                    text: 'MAD Magazine',
                    url: '/',
                },
                {
                    text: 'DC Kids',
                    url: '/',
                },
                {
                    text: 'DC Universe',
                    url: '/',
                },
                {
                    text: 'DC Power Visa',
                    url: '/',
                },
            ],
        }
    }
}
</script>

<style scoped lang='scss'>
    section {
        height: 45vh;
        background-image: url('../assets/footer-bg.jpg');
        background-size: cover;
        color: #fff;

        img {
            object-fit: cover;
            width: 50%;
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

            li:hover a {
                text-decoration: underline;
            }

             a {
                text-decoration: none;
                color: #fff;
                font-size: 10px;
            }
        }
    }
</style>