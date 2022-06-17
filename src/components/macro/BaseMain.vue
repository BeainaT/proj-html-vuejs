<template>
  <main>
    <HeroSection />
    <FounderWishes />
    <CourseSection />
    <BookSection />
    <HighLights/>
    <CounterSection/>
    <StudentsOpinion/>
  </main>
</template>

<script>
import HeroSection from '../sections/HeroSection.vue';
import FounderWishes from '../sections/FounderWishes.vue';
import CourseSection from '../sections/CourseSection.vue';
import BookSection from '../sections/BookSection.vue';
import HighLights from '../sections/HighLights.vue';
import CounterSection from '../sections/CounterSection.vue';
import StudentsOpinion from '../sections/StudentsOpinion.vue';
export default {
    name: 'BaseMain',
    components: {
    HeroSection,
    FounderWishes,
    CourseSection,
    BookSection,
    HighLights,
    CounterSection,
    StudentsOpinion
}
}
</script>

<style>

</style>