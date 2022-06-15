<template>
  <main>
    <HeroSection />
    <FounderWishes />
  </main>
</template>

<script>
import HeroSection from '../sections/HeroSection.vue';
import FounderWishes from '../sections/FounderWishes.vue';
export default {
    name: 'BaseMain',
    components: {
    HeroSection,
    FounderWishes
}
}
</script>

<style>

</style>