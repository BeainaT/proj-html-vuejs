<template>
  <div class="col-3">
    <h5>about</h5>
    <p>
        <a href="#">MasterStudy</a> is Education WordPress theme featured by Learning Menagement System (LMS) for online education. Developed by <a href="#">StylemixThemes</a>.
    </p>
    <div class="col-4 d-flex justify-content-between icon">
        <i v-for="(social, i) in footerSocial" :class="social" :key="'social' + i"></i>
    </div>
  </div>
</template>

<script>
export default {
    name: 'AboutFooter',
    data() {
        return {
            footerSocial: [
                `fa-brands fa-facebook`,
                `fa-brands fa-twitter`,
                `fa-brands fa-instagram`
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    a {
        color: #010158;
    }
    .icon {
        font-size: 1.25rem;
    }

</style>