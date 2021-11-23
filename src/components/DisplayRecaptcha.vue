<template>
  <vue-recaptcha
      sitekey="6Lc0mkQdAAAAAAy2wzBniXg8zGFNDsu_Gv_mKsxn"
      @verify="successVerify"
  >

  </vue-recaptcha>
</template>

<script>
import VueRecaptcha from 'vue-recaptcha';
export default {
  name: "DisplayRecaptcha",
  components: { VueRecaptcha },
  methods: {
    successVerify( response ) {
      console.log(response)
    }
  }
};
</script>

<style scoped>

</style>