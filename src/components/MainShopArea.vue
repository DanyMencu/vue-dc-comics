<template>
  <section>
      <div class="container d-flex">
          <a class="d-flex i-center c-center" href="/">
                <img src="@/assets/buy-comics-digital-comics.png" alt="Digital comics img">
                <span>Digital comic</span>
          </a>
          <a class="d-flex i-center c-center" href="/">
                <img src="@/assets/buy-comics-merchandise.png" alt="Merchandise comics img">
                <span>DC Merchandise</span>
          </a>
          <a class="d-flex i-center c-center" href="/">
                <img src="@/assets/buy-comics-subscriptions.png" alt="Subscriptions comics img">
                <span>Subscriptions</span>
          </a>
          <a class="d-flex i-center c-center" href="/">
                <img src="@/assets/buy-comics-shop-locator.png" alt="Shop locator img">
                <span>Comic shop locator</span>
          </a>
          <a class="d-flex i-center c-center" href="/">
                <img src="@/assets/buy-dc-power-visa.svg" alt="Shop locator img">
                <span>DC power visa</span>
          </a>
      </div>
  </section>
</template>

<script>
export default {
    name: 'MainNav',
}
</script>

<style scoped lang='scss'>
      section {
            background-color: #0282f9;

            a {
                  width: calc(100%/ 5);
                  text-decoration:  none;
                  color: #fff;
                  font-weight: 600;
                  font-size: 14px;
                  cursor: default;
                  transition: background-color 0.4s;


                  img {
                        height: 27%;
                        cursor: pointer;
                        transition: transform 0.4s;
                  }

                  span {
                        padding-left: 0.5rem;
                        cursor: pointer;
                        transition: transform 0.4s;
                  }
                  &:hover img,
                  &:hover span {
                        transform: scale(1.1);
                  }

                  &:hover {
                        background-color: #198ffd;
                  }


            }
      }
</style>