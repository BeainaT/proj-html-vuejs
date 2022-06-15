<template>
  <nav class="nav_links">
    <ul class="d-flex p-0 m-0">
      <li v-for="(link, i) in navLinks.headerLinks" :key="'link' + i"><a href="#">{{link.name}}</a></li>
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

    li {
      padding: 0 1.25rem;
      font-weight: bold;
      text-transform: capitalize;
    }

</style>