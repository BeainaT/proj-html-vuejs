<template>
  <main>
    <HeroSection />
    <FounderWishes />
    <CourseSection />
    <BookSection />
  </main>
</template>

<script>
import HeroSection from '../sections/HeroSection.vue';
import FounderWishes from '../sections/FounderWishes.vue';
import CourseSection from '../sections/CourseSection.vue';
import BookSection from '../sections/BookSection.vue';
export default {
    name: 'BaseMain',
    components: {
    HeroSection,
    FounderWishes,
    CourseSection,
    BookSection
}
}
</script>

<style>

</style>