<script>
import Footer from '@components/Footers/Footer.vue'
import NavBar from '@components/Navbar/Navbar.vue'

export default {
  components: { Footer, NavBar },
}
</script>

<template>
  <div>
    <NavBar />
    <div class="container lg:mx-auto">
      <slot />
    </div>
    <Footer />
  </div>
</template>

<style lang="scss" module>
@import '@design';

.container {
  min-width: $size-content-width-min;
  max-width: $size-content-width-max;
  margin: 0 auto;
}
</style>
