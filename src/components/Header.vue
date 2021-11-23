<template>
  <section>
      <div class="container d-flex s-between">
            <a href="/">
                <img  class="header-logo" src="@/assets/dc-logo.png" alt="DC logo">
            </a>
            <ul class="d-flex i-center">
                <li v-for="(element, index) in headerLink" :key="`link-${index}`">
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
        margin: 15px 0;
    }

    .container > a {
        height: 100%;
    }

        .header-logo {
        height: 100%;
        padding: 0.25rem;
        transition: transform 1.75s;

        &:hover {
            transform: rotateY(360deg);
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
            transition: transform 0.2s;

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
            height: 3px;
        }

        li a.active,
        li:hover a {
            color: #0b5ba5;
            transform: scale(1.05);
        }
    }

</style>