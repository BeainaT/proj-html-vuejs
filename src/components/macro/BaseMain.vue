<template>
  <main>
    <HeroSection />
    <FounderWishes />
    <CourseSection />
  </main>
</template>

<script>
import HeroSection from '../sections/HeroSection.vue';
import FounderWishes from '../sections/FounderWishes.vue';
import CourseSection from '../sections/CourseSection.vue';
export default {
    name: 'BaseMain',
    components: {
    HeroSection,
    FounderWishes,
    CourseSection
}
}
</script>

<style>

</style>