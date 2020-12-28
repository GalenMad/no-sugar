<template>
  <div>
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
            <div class="card-price-and-button">
            <p class="card-price">
              {{ item.price }} ₽
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
import image4 from '../assets/content-images/promo/image-4.jpg'
import image5 from '../assets/content-images/promo/image-5.jpg'
import image6 from '../assets/content-images/promo/image-6.jpg'
export default {
  data () {
    return {
      catalog: [
        {
          name: "Тарталетка 'Зеленое яблоко'",
          description:
            'Тарталетка с яблочным муссом, компоте из зелёных яблок и фисташковым бисквитом пропитанным соком юдзу',
          badgeList: ['Популярный десерт'],
          price: 350,
          img: image1
        },
        {
          name: "Пирожное 'Три Шоколада'",
          description:
            'Пирожное состоящее из слоёв шоколадного мусса с шоколадным бисквитом дакуаз на хрустящем кранче из тёмного шоколада с орехом пекан. Покрывается чёрной глазурью.',
          badgeList: ['Популярный десерт', 'Пониженное содержание сахара'],
          price: 320,
          img: image2
        },
        {
          name: "Торт 'Инжир-клубника-малина'",
          description:
            'Мусс из садового инжира с компоте из клубники, малиновым конфитюром, на безглютеновом бисквите и кокосовым крамблом, покрытые малиновой глазурью.\n* в основе этого десерта фрукты и ягоды, которые мы вырастили для Вас в собственных садах, в городе Сочи.',
          badgeList: ['Популярный десерт', 'Из нашего сада', 'Без глютена'],
          price: 1900,
          img: image3
        },
        {
          name: 'Пряный тарт с мандарином',
          description:
            'Взбитый пряный ганаш с компоте из мандарина и листьев лайма на фисташковом бисквите в тарталетке на основе миндальной муки.',
          badgeList: ['Популярный десерт'],
          price: 390,
          img: image4
        },
        {
          name: 'Банановое полено с мускатным орехом',
          description:
            'Нежный банановый мусс с мускатным орехом, компоте из ягод малины и клубники. В основе- морковный бисквит. ',
          badgeList: ['Популярный десерт', 'Шикарное полено!', 'Непревзойдённый банан!'],
          price: 2100,
          img: image5
        },
        {
          name: 'Торт малина-манго-кокос',
          description:
            'Веганский малиновый мусс с кремю из манго и мармеладом из кокоса на кокосово-миндальном бисквите.',
          badgeList: ['100% VEGAN', 'Фитнес-меню', 'Без глютена', 'Пониженное содержание сахара'],
          price: 2100,
          img: image6
        }
      ]
    }
  }
}
</script>
<style scoped>
.card {
  margin-top: 30px;
  min-height: 645px;
}
h2 {
  text-align: center;
}
.card-body {
  display: flex;
  flex-direction: column;
}
.btn-primary {
  width: 100%;
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
}
.card-price {
  color: #0d6efd;
  font-size: 24px;
}
.card-price-and-button{
  margin-top: auto;
}

</style>
