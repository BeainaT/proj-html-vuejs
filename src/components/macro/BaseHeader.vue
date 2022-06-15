<template>
  <header>
    <div class="container d-flex justify-content-around py-4">
      <HeaderLogo />
      <HeaderRight/>
    </div>
    <HeroSection />
  </header>
</template>

<script>
import HeaderLogo from '../commons/HeaderLogo.vue';
import HeaderRight from '../sections/HeaderRight.vue';
import HeroSection from '../sections/HeroSection.vue';
export default {
    name: "BaseHeader",
    components: {
    HeaderLogo,
    HeaderRight,
    HeroSection
}
}
</script>

<style>

</style>