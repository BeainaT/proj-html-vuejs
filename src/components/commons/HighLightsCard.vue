<template>
  <div class="why_cards d-flex align-items center col-5">
    <div class="row justify-content-evenly">
        <div class="col-2 icon_col py-5">
            <span><i :class="best.icon"></i></span>
        </div>
        <div class="col-9 details_col py-5">
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
        &:hover {
            background-color: var(--primary_color);
            & p {
                color: var(--text_body);
            }
            & .icon_col .icons {
                color: var(--secondary_color)
            }
        }
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