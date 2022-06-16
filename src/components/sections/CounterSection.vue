<template>
  <section class="d-flex justify-content-center align-items-center">
      <div class="container d-flex justify-content-around">
    <CounterElements v-for="(count, i) in counter" :key="'count' + i" :count="count"/>
    </div>
  </section>
</template>

<script>
import CounterElements from '../commons/CounterElements.vue';
export default {
    name: 'CounterSection',
    components: {
    CounterElements
    },
    data() {
        return {
            counter: [
                {
                    number: 3195,
                    icon: `fa-solid fa-user-group`,
                    title: "Online learner"
                },
                {
                    number: 23,
                    icon: `fa-solid fa-film`,
                    title: "Video Courses"
                },
                {
                    number: 437,
                    icon: `fa-regular fa-image`,
                    title: "Sliders & Images"
                },
                {
                    number: 1440,
                    icon: `fa-regular fa-thumbs-up`,
                    title: "Excellent Reviews"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    section {
        background-image: url("../../assets/img/counter-1919x1101.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        color: var(--secondary_color);
        min-height: 34.375rem;
    }
</style>