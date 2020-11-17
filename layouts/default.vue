<template>
  <div>
    <Header/>
    <Nuxt />
    <Footer/>
  </div>
</template>

<style>
@import '../styles/global.scss';
</style>
<script>

  import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'
export default {
  components: {
    Header, Footer
}
}
</script>