<template>
  <div class="container subscribe_box">
    <div class="row py-5 justify-content-evenly">
        <div class="col-6">
          <SubForm />
        </div>
        <div class="col-5 counter">
          <SubCounter />
        </div>
    </div>
  </div>
</template>

<script>
import SubForm from '../commons/SubForm.vue'
import SubCounter from '../commons/SubCounter.vue'

export default {
    name: 'SubscribeSection',
    components: {
    SubForm,
    SubCounter
}
}
</script>

<style lang="scss" scoped>
  .subscribe_box {
    background-color: var(--primary_color);
    border-radius: .625rem;
    position: relative;
    bottom: 9.375rem;
    .counter {
      text-align: center;
    }
  }

</style>