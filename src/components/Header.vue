<template>
  <header>
    <div class="container">
      <div class="row d-flex">
        <div class="col">
          <div class="d-flex">
            <div class="col">
              <img src="../assets/images/logo-desktop.png" alt="">
            </div>
            <div class="col">
              <Button text="карта" />
            </div>
          </div>
        </div>
        <div class="col">

        </div>
      </div>
    </div>
  </header>
</template>

<script>
import Button from './Button'
export default {
  name: "Header",
  components: {
    Button
  }
}
</script>

<style lang="scss">
  header {
    padding-top: 18px;
    .row {
      justify-content: space-between;
      .btn {

      }
    }
  }
</style>
