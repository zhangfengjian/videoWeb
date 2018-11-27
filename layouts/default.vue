<template>
  <div>
    <Top/>
    <nuxt/>
    <Footer/>
  </div>
</template>
<script>
  import Top from "~/components/Top.vue"
  import Footer from "~/components/Footer.vue"
  export default {
    components: {
      Top,
      Footer
    }
  }
</script>
<style>

</style>
