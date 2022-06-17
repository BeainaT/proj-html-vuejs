<template>
  <div class="col-3">
    <h4>pages</h4>
    <div class="row">

        <ul class="col-6" v-for="pageLink in pageLinks" :key="pageLink">
            <li>{{pageLink}}</li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
    name: 'PagesFooter',
    data() {
        return {
            pageLinks: [
                'blog',
                'courses',
                'home',
                'membership a...',
                'shortcodes',
                'typography'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
ul li {
    list-style: disc;
    text-transform: capitalize;
    margin-left: 1rem;
}

</style>