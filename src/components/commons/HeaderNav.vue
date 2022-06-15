<template>
  <nav class="nav_links">
    <ul class="d-flex p-0 m-0">
      <li v-for="link in navLinks.headerLinks" :key="link"><a href="#">{{link.name}}</a></li>
    </ul>
  </nav>
</template>

<script>
import navLinks from '../shared/navLinks'
export default {
    name: 'HeaderNav',
    data() {
      return {
        navLinks
      }
    }
}
</script>

<style lang="scss" scoped>

  .nav_links {
    font-family: var(--typo_serif);
      li {
        padding: 0 1.25rem;
        font-weight: bold;
        text-transform: capitalize;
      }
    }

</style>