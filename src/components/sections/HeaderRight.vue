<template>
  <div class="header_right d-flex justify-content-end align-items-center">
    <HeaderNav />
    <HeaderSocial />
  </div>
</template>

<script>
import HeaderNav from '../commons/HeaderNav.vue'
import navLinks from '../shared/navLinks'
import HeaderSocial from '../commons/HeaderSocial.vue'
export default {
  name: 'HeaderRight',
  components: {
    HeaderNav,
    HeaderSocial
},
  data() {
    return {
      navLinks
    }
  }
}
</script>

<style lang="scss" scoped>
  .header_right {
    gap: 1.25rem;
    color: var(--text_nav);
  }
</style>