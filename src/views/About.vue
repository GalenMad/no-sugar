<template>
  <div>
    <app-promo/>
  </div>
</template>
<script>
import Promo from '../components/Promo.vue'
export default {
  props: Array,
  components: {
    appPromo: Promo
  }
}
</script>
