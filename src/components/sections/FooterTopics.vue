<template>
  <div class="container">
    <div class="row">
        <div class="col-3" v-for="title in footerTitles" :key="title"><h4>{{title}}</h4>
        </div>
        <div class="row">
            <AboutFooter/>
            <ContactFooter/>
            <PagesFooter />
            <BlogFooter />
        </div>
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
    data() {
        return {
            footerTitles : [
                'about',
                'contact',
                'pages',
                'blog'
            ]
        }
    }
}
</script>

<style>

</style>