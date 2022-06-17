<template>
  <div class="col-3">
    <h5>contact</h5>
    <div class="contact_font" v-for="(contact, i) in contacts" :key="'contact' + i">
        <address>{{contact.adress}}</address>
        <address>Tel.: {{contact.phone}} <br> Fax: {{contact.fax}}</address>
        <small>{{contact.mail}}</small>
    </div>

  </div>
</template>

<script>
export default {
    name: 'ContactFooter',
    data() {
        return {
            contacts: [
                {
                    adress: 'USA, California 20, First Avenue, California',
                    phone: '+1 212 458 300 32',
                    fax: '+1 212 375 24 14',
                    mail: 'info@masterstudy.com'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.contact_font {
    font-family: var(--typo_sans_serif);
}

</style>