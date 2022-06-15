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
      &:nth-child(3) {
        position: relative;
      }
      &:nth-child(3)::after {
        content:"NEW";
        background-color: var(--news_badge);
        color: var(--secondary_color);
        border-radius: .3125rem .3125rem .3125rem 0;
        font-size: .625rem;
        padding: .125rem .25rem;
        position: absolute;
        bottom: 1.2rem;
        right: 0.5rem;
      }
      a {
        padding-bottom: 0.5rem;
        &:hover {
          border-bottom: .1875rem solid var(--primary_color);
          position: relative;
          &::after {
            content: "";
            width: 0;
            height: 0;
            border-left: .1875rem solid transparent;
            border-right: .1875rem solid transparent;
            border-bottom: .1875rem solid var(--primary_color);
            position: absolute;
            bottom: 0;
            left: calc(50% - .0938rem);
          }
        }
      }
    }

</style>