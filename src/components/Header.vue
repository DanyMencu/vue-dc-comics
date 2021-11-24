<template>
  <section>
      <div class="container d-flex s-between">
            <a class="header-logo" href="/">
                <img   src="@/assets/dc-logo.png" alt="DC logo">
            </a>
            <ul class="d-flex i-center">
                <li class="d-flex i-center" v-for="(element, index) in headerLink" :key="`link-${index}`">
                    <a :class="{ active: element.current}" :href="element.url">{{ element.text }}</a>
                </li>
            </ul>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            headerLink: [
                {
                    text: 'Characters',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Movies',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Tv',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '/',
                    current: false,
                },
                {
                    text: 'News',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Characters',
                    url: '/',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '/',
                    current: false,
                },
            ]
        }
    }
}
</script>

<style scoped lang='scss'>
    
    section {
        height: 10vh;
    }

    .container > a {
        height: 100%;
    }

        .header-logo {
        height: 100%;
        padding: 0.7rem 0;
        transition: transform 1.75s;

        &:hover {
            transform: rotateY(360deg);
            filter:contrast(120%);
        }

        img {
            height: 100%;
        }
    }

    ul {
        height: 100%;
        justify-content: center;
        list-style: none;

        li {
            height: 100%;
            margin: 0 0.6rem;
            border-bottom: 3px solid #0b5ba500;
            transition: border-bottom 0.15s;

            &:hover {
                border-bottom: 3px solid #0b5ba5;
            }

            a {
                display: inline-block;
                text-decoration: none;
                color: #000;
                text-transform: uppercase;
                font-size: 14px;
                font-weight: 600;
                transition: transform 0.2s;

            }
        }

        li a.active,
        li:hover a {
            color: #0b5ba5;
            transform: scale(1.05);
        }
    }

</style>