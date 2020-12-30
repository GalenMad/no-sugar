<template>
    <div class="row">
      <div class="col-sm-12 col-lg-6">
        <h3 class="text-left">Как сделать заказ персонального десерта?</h3>
        <ol>
          <li>Заполните форму справа</li>
          <li>Мы перезвоним вам, запишем все ваши пожелания и оформим заказ</li>
          <li>Оплатите и заберите свой тортик/конфеты/всё, что угодно!</li>
        </ol>
      </div>
      <div class="col-sm-12 col-lg-6">
        <form>
          <div class="form-group">
            <label for="inputName">Ваше имя</label>
            <input type="text" class="form-control" id="inputName" />
          </div>
          <div class="form-group">
            <label for="inputTel">Телефон</label>
            <input type="tel" class="form-control" id="inputTel" />
            <small id="telHelp" class="form-text text-muted"
              >Мы не будем рассылать вам спам или рекламные предложения.</small
            >
          </div>
          <div class="form-group form-check">
            <input
              type="checkbox"
              class="form-check-input"
              id="exampleCheck1"
            />
            <label class="form-check-label" for="exampleCheck1"
              >Я согласен на обработку персональных данных</label
            >
          </div>
          <button type="submit" class="btn btn-primary">Отправить</button>
        </form>
      </div>
    </div>
</template>

<script>
export default {

}
</script>
<style scoped>
h2 {
  font-weight: bold;
}
.form-group {
  width: 50%;
  margin-right: auto;
  margin-left: auto;
  text-align: left;
  margin-bottom: 10px;
}
.card {
  width: auto;
  margin-right: auto;
  margin-left: auto;
  display: inline-flex;
  margin-bottom: 30px;
  justify-content: space-around;
}
.btn {
  width: 40%;
  margin-bottom: 10px;
}
.form-check-label {
  text-align: left;
  font-size: 90%;
}
li{
  text-align: left;
  font-weight: bold;
  font-size: 130%;
}
</style>
