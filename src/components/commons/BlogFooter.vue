<template>
  <div class="col-3">
    <h5>blog</h5>
    <div class="row gy-3">
        <div class="col-12 d-flex" v-for="(blogLink, i) in blogLinks" :key="'blogLink' + i">
        <div class="row align-items-end">
            <div class="col-4">
                <img :src="blogLink.img" alt="article img">
            </div>
            <div class="col-8">
                <div class="row">
                    <div class="col-12">
                        <h6>{{blogLink.title}}</h6>
                    </div>
                    <div class="col-12">
                        <small>&mdash;{{blogLink.date}}</small>
                    </div>
                </div>
            </div>
        </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'BlogFooter',
    data() {
        return {
            blogLinks: [
                {
                    img: require('../../assets/img/photo-1517520287167-4bbf64a00d66-69x69.jpeg'),
                    title: `Our main target is to "Developing Yourself as a Leader"`,
                    date: "August 9, 2018", 
                },
                {
                    img: require('../../assets/img/photo-1490376840453-5f616fbebe5b-69x69.jpeg'),
                    title: `Those Other College, Expenses You Aren't Thinking About`,
                    date: "June 3, 2015", 
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    img {
        width: 100%;
        transform: scale(0.9);
    }
    h6 {
        margin-bottom: 0;
    }
    small {
        font-family: var(--sans_serif);
        color: #808080;
    }
</style>