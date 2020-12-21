<template>
  <div>
    <div class="container">
      <h2>Акции</h2>
      <div class="row">
          <div
            class="col-12 col-sm-6 col-lg-4 d-flex"
            v-for="item in catalog"
            :key="item.index"
          >
            <div class="card">
              <img :src="item.img" class="card-img-top" :alt="item.name" />
              <div class="card-body">
                <h5 class="card-title">{{ item.name }}</h5>
                <div class="mb-3 bagdes">
                <span
                  class="badge bg-primary"
                  v-for="badge in item.badgeList"
                  :key="badge.index"
                  >{{ badge }}</span
                >
                </div>
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
import image1 from '../assets/content-images/promo/image-1.jpg'
import image2 from '../assets/content-images/promo/image-2.jpg'
import image3 from '../assets/content-images/promo/image-3.jpg'
export default {
  data () {
    return {
      catalog: [
        {
          name: "Тарталетка 'Зеленое яблоко'",
          description:
            'Тарталетка с яблочным муссом, компоте из зелёных яблок и фисташковым бисквитом пропитанным соком юдзу',
          badgeList: ['Популярный десерт'],
          img: image1
        },
        {
          name: "Пирожное 'Три Шоколада'",
          description:
            'Пирожное состоящее из слоёв шоколадного мусса с шоколадным бисквитом дакуаз на хрустящем кранче из тёмного шоколада с орехом пекан. Покрывается чёрной глазурью.',
          badgeList: ['Популярный десерт', 'Пониженное содержание сахара'],
          img: image2
        },
        {
          name: "Торт 'Инжир-клубника-малина'",
          description:
            'Мусс из садового инжира с компоте из клубники, малиновым конфитюром, на безглютеновом бисквите и кокосовым крамблом, покрытые малиновой глазурью.\n* в основе этого десерта фрукты и ягоды, которые мы вырастили для Вас в собственных садах, в городе Сочи.',
          badgeList: ['Популярный десерт', 'Из нашего сада', 'Без глютена'],
          img: image3
        }
      ]
    }
  }
}
</script>
<style scoped>
h2 {
  text-align: center;
}
div.col-4 {
  display: flex;
}
.card-body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.btn-primary {
  width: 100%;
  align-self: flex-end;
}
.card-img-top {
  max-height: 255px;
}
.badge {
  margin: 8px;
  padding: 8px;
  text-transform: uppercase;
}
.badges {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
}
</style>
