<template>
  <div>
    <div class="row">
      <div
        class="col-sm-12 col-lg-4 d-flex"
        v-for="column in about"
        :key="column.index"
      >
        <div class="card">
          <img :src="column.img" class="card-img-top" :alt="column.heading" />
          <div class="card-body">
            <h5 class="card-title">{{ column.heading }}</h5>
            <p class="card-text">
              {{ column.description }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import icon1 from '../assets/content-images/about/icon-1.svg'
import icon2 from '../assets/content-images/about/icon-2.svg'
import icon3 from '../assets/content-images/about/icon-3.svg'
export default {
  data () {
    return {
      about: [
        {
          heading: 'Качественные и вкусные продукты',
          description:
            'При производстве в Сочи у нас также есть собственный сад, в котором растут инжир, хурма, яблоки, груши и фундук, например, мы сушим яблоки и груши, замораживаем свежий инжир, замораживаем и вялим спелую хурму. Мы отбираем самые спелые ягоды и фрукты сада и привозим в Петербург в специальных рефрижераторах (морозильные установки), которые позволят в целости доставить продукт, чтоб они стали главным ингредиентом в наших десертах.',
          img: icon1
        },
        {
          heading: 'Красивые десерты',
          description:
            'Десерты должны вызывать весь спектр удовольствий и мы делаем все, чтобы они получались красивыми. ',
          img: icon2
        },
        {
          heading: 'Вкус и польза',
          description:
            '«Сахара нет» — это баланс вкуса и пользы, который мы соблюдаем за счёт употребления минимального количества сахара или полного исключения его из рецепта, а так же за счёт уменьшения калорийности, путём замены продуктов на более легкие, натуральные и полезные. В нашем меню вы найдете веганские, сыроедческие, фитнес десерты, а так же десерты без сахара и глютена.',
          img: icon3
        }
      ]
    }
  }
}
</script>
<style scoped lang="scss">
img {
  max-width: 80px;
  align-self: center;
}
.container {
  margin-bottom: 40px;
}
.card {
  padding: 10px;
  border: 3px solid #0d6efd;
  margin-bottom: 30px;

  &-title {
    font-weight: 600;
  }

  &-text {
    text-align: left;
  }
}
</style>
