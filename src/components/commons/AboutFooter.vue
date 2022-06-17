<template>
  <div class="col-3">
    <h4>about</h4>
    <p><a href="#">MasterStudy</a> is Education WordPress theme featured by Learning Menagement System (LMS) for online education. Developed by <a href="#">StylemixThemes</a>.</p>
    <i v-for="(social, i) in footerSocial" :class="social" :key="'social' + i"></i>
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

<style>

</style>