<template>
  <div class="container py-5">
        <div class="row">
            <AboutFooter/>
            <ContactFooter/>
            <PagesFooter />
            <BlogFooter />
        </div>
  </div>
</template>

<script>
import AboutFooter from '../commons/AboutFooter.vue'
import ContactFooter from '../commons/ContactFooter.vue'
import PagesFooter from '../commons/PagesFooter.vue'
import BlogFooter from '../commons/BlogFooter.vue'
export default {
    name: 'FooterTopics',
    components: {
    AboutFooter,
    ContactFooter,
    PagesFooter,
    BlogFooter
    },

}
</script>

<style lang="scss">
    h4 {
        text-transform: uppercase;
    }

</style>