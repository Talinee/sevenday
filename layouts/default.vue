<template>
  <div>
    <header-bar/>
    <Nuxt />
    <footer-bar/>
  </div>
</template>

<style>
@import '../styles/global.scss';
</style>
<script>

  import HeaderBar from '../components/HeaderBar.vue'
import FooterBar from '../components/FooterBar.vue'
export default {
  components: {
    HeaderBar, FooterBar
}
}
</script>