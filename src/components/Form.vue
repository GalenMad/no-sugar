<template>
  <div>
    <div class="row">
      <div class="card">
        <h2>Напишите нам и мы вам перезвоним !</h2>
        <form class="order-form">
          <div class="form-group">
            <label for="exampleInputName">Ваше имя</label>
            <input type="text" class="form-control" id="exampleInputName" />
          </div>
          <div class="form-group">
            <label for="exampleInputPhone">Телефон</label>
            <input type="tel" class="form-control" id="exampleInputTel" />
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
  </div>
</template>
<script>
export default {}
</script>
<style scoped lang="scss">
h2 {
  font-weight: bold;
}

.order-form {
min-width: 400px;
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
  min-height: 300px;
  margin-bottom: 30px;
  justify-content: space-around;
}
.btn {
  width: 45%;
  margin-bottom: 10px;
}
.form-check-label {
  text-align: left;
  font-size: 90%;
}
</style>
