<template>
  <header>
    <div class="container">
      <div class="row d-flex">
        <div class="col">
          <div class="d-flex row-1">
            <div class="col">
              <img src="../assets/images/logo-desktop.png" alt="">
            </div>
            <div class="col">
              <a target="_blank" href="https://www.google.com.ua/maps/">
                <Button :active="true" data-text="карта" text="карта" />
              </a>
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
      .row-1 {
        justify-content: space-between;
        width: 340px;
      }
    }
  }
</style>
