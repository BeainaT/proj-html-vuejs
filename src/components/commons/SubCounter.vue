<template>
  <div class="row">
    <div class="col-3">
        <span>26</span>
        <br>
        <span>days</span>
    </div>
    <div class="col-3">
        <span>01</span>
        <br>
        <span>hours</span>
    </div>
    <div class="col-3">
        <span>47</span>
        <br>
        <span>minutes</span>
    </div>
    <div class="col-3">
        <span>31</span>
        <br>
        <span>seconds</span>
    </div>
  </div>
</template>

<script>
export default {
    name: 'SubCounter'
}
</script>

<style lang="scss" scoped>
    
    span:first-child {
        font-size: 3.2rem;
        font-weight: bold;
        color: var(--secondary_color);
    }
    span:last-child {
        text-transform: capitalize;
        font-weight: bold;
    }

</style>