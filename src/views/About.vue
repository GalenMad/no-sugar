<template>
  <div>
    <app-promo/>
    <app-form/>
  </div>
</template>
<script>
import Promo from '../components/Promo.vue'
import Form from '../components/Form.vue'
export default {
  props: Array,
  components: {
    appPromo: Promo,
    appForm: Form
  }
}
</script>
