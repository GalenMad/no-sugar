<template>
  <div class="container">
    <h2>Акции</h2>
    <app-promo/>
    <h2>Закажите десерт своей мечты!</h2>
    <app-order/>
    <h2>О нас</h2>
    <app-about/>
    <app-form/>
  </div>
</template>
<script>
import Promo from '../components/Promo.vue'
import Form from '../components/Form.vue'
import About from '../components/aboutUs.vue'
import Order from '../components/Order.vue'
export default {
  components: {
    appPromo: Promo,
    appForm: Form,
    appAbout: About,
    appOrder: Order
  }
}
</script>
<style>
.row {
  margin-bottom: 30px;
}
h2 {
  text-align: center;
}
</style>
