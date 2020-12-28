<template>
  <div>
    <h2>Напишите нам и мы вам перезвоним !</h2>
      <div class="row">
        <div class="card">
          <form>
            <div class="form-group">
              <label for="exampleInputName">Ваше имя</label>
              <input type="text" class="form-control" id="exampleInputName" />
            </div>
            <div class="form-group">
              <label for="exampleInputPhone">Телефон</label>
              <input type="tel" class="form-control" id="exampleInputTel" />
              <small id="telHelp" class="form-text text-muted"
                >Мы не будем рассылать вам спам или рекламные
                предложения.</small
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
<style scoped>
h2 {
  margin-top: 50px;
  text-align: center;
}
.form-group {
  width: 30%;
  margin-right: auto;
  margin-left: auto;
}
.card {
  width: 90%;
  margin-right: auto;
  margin-left: auto;
  display: flex;
  min-height: 300px;
  margin-bottom: 30px;
  justify-content: space-around;
}
.btn {
  width: 20%
}

</style>
