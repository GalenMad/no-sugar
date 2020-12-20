<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-4" v-for="item in catalog" :key="item.index">
          <div class="card" style="width: 18rem">
            <img :src="item.img" class="card-img-top" :alt="item.name" />
            <div class="card-body">
              <h5 class="card-title">{{ item.name }}</h5>
              <p class="card-text">
                {{ item.description }}
              </p>
              <a href="#" class="btn btn-primary">Купить</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Catalog from '../App.vue'
export default {
  catalog: Catalog
}
</script>
