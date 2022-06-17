<template>
  <footer>
    <small>
      <FooterTopics/>
    </small>
  </footer>
</template>

<script>
import FooterTopics from '../sections/FooterTopics.vue';
export default {
    name: 'BaseFooter',
    components: {
    FooterTopics
    }
}
</script>

<style lang="scss" scoped>
footer {
  background-color: var(--primary_color);
  color: var(--text_nav);
  font-weight: 300;
}

</style>