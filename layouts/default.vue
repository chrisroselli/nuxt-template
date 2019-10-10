<template>
  <div>
    <TopNav />
    <HomeSlider />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import TopNav from '~/components/TopNav.vue'
import HomeSlider from '~/components/HomeSlider.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    TopNav,
    HomeSlider,
    Footer
  }
}
</script>

