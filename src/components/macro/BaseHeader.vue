<template>
  <header>
    <div class="container d-flex justify-content-around py-4">
      <HeaderLogo />
      <HeaderRight/>
    </div>
  </header>
</template>

<script>
import HeaderLogo from '../commons/HeaderLogo.vue';
import HeaderRight from '../sections/HeaderRight.vue';

export default {
    name: "BaseHeader",
    components: {
    HeaderLogo,
    HeaderRight,
}
}
</script>

<style>

</style>