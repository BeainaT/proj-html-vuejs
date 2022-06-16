<template>
    <div class="row">
        <div class="col-12">
            <h3><span>limited sale:</span> All courses with 55% off</h3>
            </div>
        <form class="col-12">
            <input type="text" placeholder="Enter your E-mail">
            <button>subscribe</button>
        </form>
    </div>
</template>

<script>
export default {
    name: 'SubForm'
}
</script>

<style lang="scss" scoped>
h3 {
    margin-bottom: 2rem;
    font-weight: bold;
    span {
        color: var(--secondary_color);
        text-transform: capitalize;
    }
}
form {
    position: relative;
    
    input {
        width: 100%;
        font-family: var(--typo_sans_serif);
        box-shadow: 0 .0625rem .3125rem #8b8b8b;
        &:focus {
            outline: none;
        }
    }
    button {
        position: absolute;
        right: 0;
        background-color: var(--bg_submit);
    }
}

</style>