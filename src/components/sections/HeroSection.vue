<template>
    <section class="hero_section">
        <img src="../../assets/img/slide-1.jpg" alt="">
        <SloganTitle />
        <SubscribeSection />
    </section>
</template>


<script>
import SloganTitle from '../commons/SloganTitle.vue'
import SubscribeSection from './SubscribeSection.vue'
export default {
    name: 'HeroSection',
    components: {
    SloganTitle,
    SubscribeSection
},
}
</script>

<style lang="scss">
    .hero_section {
        position: relative;
        img {
            width: 100%;
        }
    }
</style>