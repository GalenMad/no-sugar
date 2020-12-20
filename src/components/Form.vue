<template>
  <div>
    <div class="container">
      <div class="row">
        <form>
          <div class="form-group">
            <label for="exampleInputname">Email address</label>
            <input type="text" class="form-control" id="exampleInputname" />
          </div>
          <div class="form-group">
            <label for="exampleInputPhone">Password</label>
            <input type="phone" class="form-control" id="exampleInputPhone" />
            <small id="phoneHelp" class="form-text text-muted"
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
          <button type="submit" class="btn btn-primary">Submit</button>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>
