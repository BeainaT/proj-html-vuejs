<template>
  <section class="container py-5">
    <h2>Why my Courses?</h2>
    <div class="row py-5 justify-content-between">
        <HighLightsCard v-for="(best, i) in bests" :key="'best' + i" :best="best"/>
    </div>
  </section>
</template>

<script>
import HighLightsCard from '../commons/HighLightsCard.vue'
export default {
    name: "HighLihts",
    components: { 
        HighLightsCard 
    },
    data() {
        return {
            bests: [
                {
                    name: "Enterpreneurship",
                    icon: `fa-solid fa-briefcase icons`,
                    details: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Delectus quidem nobis molestiae veritatis dolorem suscipit velit at autem non blanditiis, magnam totam error tempore dignissimos consequatur neque ab. Dignissimos, officiis."
                },
                {
                    name: "Accelerated learning",
                    icon: `fa-solid fa-rocket icons`,
                    details: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Delectus quidem nobis molestiae veritatis dolorem suscipit velit at autem non blanditiis, magnam totam error tempore dignissimos consequatur neque ab. Dignissimos, officiis."
                },
                {
                    name: "Productivity",
                    icon: `fa-solid fa-thumbs-up icons`,
                    details: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Delectus quidem nobis molestiae veritatis dolorem suscipit velit at autem non blanditiis, magnam totam error tempore dignissimos consequatur neque ab. Dignissimos, officiis."
                },
                {
                    name: "Life Coaching",
                    icon: `fa-solid fa-gear icons`,
                    details: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Delectus quidem nobis molestiae veritatis dolorem suscipit velit at autem non blanditiis, magnam totam error tempore dignissimos consequatur neque ab. Dignissimos, officiis."
                },
            ]
        };
    },
}
</script>

<style lang="scss" scoped>
h2 {
    text-align: center;
}
.row {
    gap: 1.5625rem;
}

</style>