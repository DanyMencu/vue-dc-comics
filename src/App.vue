<template>
  <div id="app">

    <Header />

    <main>
      <MainContent />
    </main>

    <footer>
      <FooterLink />

      <FooterSocials />
    </footer>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import MainContent from '@/components/MainContent.vue'
import FooterLink from '@/components/FooterLink.vue'
import FooterSocials from '@/components/FooterSocials.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    FooterLink,
    FooterSocials,
  }
}
</script>

<style lang="scss">
@import '@/styles/general';
@import '@/styles/utilities';
</style>
