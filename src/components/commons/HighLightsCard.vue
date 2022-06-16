<template>
  <div class="why_cards">
    <div class="row py-5">
        <div class="col-2 icon_col">
            <span><i :class="best.icon"></i></span>
        </div>
        <div class="col-9 details_col">
            <h4>{{best.name}}</h4>
            <p>{{best.details}}</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'HighLights',
    props: {
        best: Object
    }
}
</script>

<style lang="scss" scoped>
.why_cards {
    border-left: .3125rem solid var(--primary_color);
    box-shadow: .125rem .5rem 15px var(--card_secondary);
    width: calc(50% - .8125rem);
    p {
        color: var(--card_secondary);
        line-height: 1.875rem;
    }
    .icon_col {
        text-align: end;
        .icons {
            font-size: 3.125rem;
            color: var(--primary_color);
        }
    .details_col {
        padding: 0 1.25rem;
    }
    }
}
</style>