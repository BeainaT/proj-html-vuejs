<template>
  <main>
    <HeroSection />
    <FounderWishes />
    <CourseSection />
    <BookSection />
    <HighLights/>
    <CounterSection/>
  </main>
</template>

<script>
import HeroSection from '../sections/HeroSection.vue';
import FounderWishes from '../sections/FounderWishes.vue';
import CourseSection from '../sections/CourseSection.vue';
import BookSection from '../sections/BookSection.vue';
import HighLights from '../sections/HighLights.vue';
import CounterSection from '../sections/CounterSection.vue';
export default {
    name: 'BaseMain',
    components: {
    HeroSection,
    FounderWishes,
    CourseSection,
    BookSection,
    HighLights,
    CounterSection
}
}
</script>

<style>

</style>