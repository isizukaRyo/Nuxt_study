<template>
  <div class="container">
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Header from '~/components/Header.vue'
import Main from '~/components/Main.vue'
import Footer from '~/components/Footer.vue'


export default {
  components: {
    Logo,
    Header,
    Main,
    Footer
  }
}
</script>

<style>

</style>
