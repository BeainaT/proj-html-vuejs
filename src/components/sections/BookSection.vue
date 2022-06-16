<template>
  <section>
    <BookShop/>
  </section>
</template>

<script>
import BookShop from '../commons/BookShop.vue';
export default {
    name: "BookSection",
    components: { 
        BookShop 
    }
}
</script>

<style lang="scss" scoped>

    section {
        background-image: url(../../assets/img/slider_1-1917x607-1914x606.jpg);
        color: var(--secondary_color);
        text-align: center;
    }

</style>