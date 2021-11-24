<template>
  <section>
      <div class="container d-flex s-between py-1">
          <button>Sing-up now!</button>
          <div class="socials d-flex">
              <h3>Follow us</h3>
              <a v-for="(element, index) in Socials" :key="`socialsIndex-${index}`" :href="element.url">
                <img :src="element.img" :alt="`${element.text} logo`" >
              </a>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name:'FooterSocials',
    data(){
        return {
            Socials: [
                {
                    text: 'Facebook',
                    img: require('@/assets/footer-facebook.png'),
                    url: '/'
                },
                {
                    text: 'Twitter',
                    img: require('@/assets/footer-twitter.png'),
                    url: '/'
                },
                {
                    text: 'Youtube',
                    img: require('@/assets/footer-youtube.png'),
                    url: '/'
                },
                {
                    text: 'Pinterest',
                    img: require('@/assets/footer-pinterest.png'),
                    url: '/'
                },
                {
                    text: 'Periscope',
                    img: require('@/assets/footer-periscope.png'),
                    url: '/'
                },
            ],
        }
    }
}
</script>

<style scoped lang='scss'>
    section {
        background-color: #303030;

        button {
            font-weight: 600;
            color: #fff;
            text-transform: uppercase;
            padding: 0.5rem 1rem;
            background: none;
            border: 2px solid #145ea3;
            cursor: pointer;
            transition: background-color 0.3s;
            
            &:hover { 
                background: #145ea3;
            }
        }

        h3 {
            color: #145ea3;
            text-transform: uppercase;
            margin-right: 0.5rem;
            align-self: center;
        }

        img {
            height: 85%;
            margin: 0 0.5rem;
            border: 0 solid #797979;
            border-radius: 50%;
            transition: all 0.25s;

            &:hover {
                filter:brightness(170%);
                box-shadow: 0 0 10px 1px #868686;
                transform: scale(1.05);
            }
        }

    }
</style>