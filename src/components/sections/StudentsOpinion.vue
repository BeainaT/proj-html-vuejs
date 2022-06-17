<template>
  <section>
    <div class="container_small py-5">
      <h2>What students say</h2>
      <div class="container-fluid">
        <StudentsCarousel/>
          <h5 class="mb-1 mt-3">Paints of the Future</h5>
          <i class="fa-solid fa-star stars_custom" v-for="(star, i) in 5" :key="'star' + i"></i>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolor temporibus quod labore eius suscipit. Error vel voluptate doloribus eligendi dignissimos mollitia ullam earum maxime est, dolor voluptatibus, quibusdam, accusamus laudantium? Lorem ipsum dolor sit amet, consectetur adipisicing elit. Velit tempore iste dignissimos nihil dolor dolores, modi aut temporibus cumque, soluta quos sequi adipisci numquam doloremque itaque eius debitis ex reiciendis?</p>
      </div>

    </div>
  </section>
</template>


<script>
import StudentsCarousel from '../commons/StudentsCarousel.vue';
export default {
    name: 'StudentsOpinion',
    components: {
    StudentsCarousel
}
}
</script>

<style lang="scss" scoped>
  h2 {
      text-transform: capitalize;
  }
  p {
    margin: 1.25rem 0;
    line-height: 1.8rem;
  }
  .stars_custom {
    color: var(--primary_color);
    margin: 0 .1875rem;
  }

</style>