<template>
  <section>
      <div class="container d-flex s-between py-1">
          <button>Sing-up now!</button>
          <div class="socials d-flex">
              <h3>Follow us</h3>
              <a href="/">
                <img src="@/assets/footer-facebook.png" alt="Facebook logo">
              </a>
              <a href="/">
                <img src="@/assets/footer-twitter.png" alt="Twitter logo">
              </a>
              <a href="/">
                <img src="@/assets/footer-youtube.png" alt="Youtube logo">
              </a>
              <a href="/">
              
              <img src="@/assets/footer-pinterest.png" alt="Pinterest logo">
              </a>
              <a href="/">
                <img src="@/assets/footer-periscope.png" alt="Periscope logo">
              </a>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name:'FooterSocials',
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
        }

    }
</style>