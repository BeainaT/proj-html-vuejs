<template>
    <div class="elm_box align-items-center">
      <span><i :class="count.icon"></i></span>
      <div class="details">
        <span>{{count.number}}</span>
        <span>{{count.title}}</span>
      </div>
    </div>
</template>

<script>

export default {
    name: 'CounterElements',
    props: {
      count: Object
    }
}
</script>

<style lang="scss" scoped>
  .elm_box {
    display: flex;
    width: 20%;
    justify-content: space-evenly;
    span:first-child {
      font-size: 4rem;
    }
    span:last-child {
      font-weight: 400;
      font-size: 1.25rem;
    }
    .details {
      display: flex;
      flex-direction: column;
      span:first-child {
        color: var(--yellow_counters);
        font-weight: bold;
        font-size: 2.5rem;
      }
    }
  }
</style>