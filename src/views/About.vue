<template>
  <div class="container">
    <app-promo/>
    <app-form/>
    <app-about/>
  </div>
</template>
<script>
import Promo from '../components/Promo.vue'
import Form from '../components/Form.vue'
import About from '../components/aboutUs.vue'
export default {
  props: Array,
  components: {
    appPromo: Promo,
    appForm: Form,
    appAbout: About
  }
}
</script>
<style>
.row {
  margin-bottom: 30px;
}
</style>
