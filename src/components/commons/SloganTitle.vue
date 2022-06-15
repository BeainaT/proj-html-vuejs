<template>      
  <div class="slogan_box">  
        <h1>Start your Human <span>Revolution</span> today</h1>
        <p class="py-2">A wonderful serenity has taken possession of my entire soul, like these sweet mornings of spring which I enjoy with my whole heart.</p>  
  </div>
</template>

<script>
export default {
  name: 'SloganTitle'
}
</script>

<style lang="scss" scoped>
  .slogan_box {
    position: absolute;
    top: 20%;
    left: 50%;
    max-width: 31.25rem;
    & > h1 span {
      color: var(--primary_color);
    }
    & > p {
      font-family: var(--typo_sans_serif);
    }
  }
</style>