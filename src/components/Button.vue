<template>
  <button class="btn">{{ text }}</button>
</template>

<script>
export default {
  name: "Header",
  props: {
    text: String
  }
}
</script>

<style lang="css">
  .btn {
    text-transform: uppercase;
    border-width: 3px;
    border-color: rgb(93, 93, 93);
    border-style: solid;
    background-color: rgb(101, 156, 193);
    width: 97px;
    height: 38px;
    font-weight: 300;
    color: #ffffff;
    font-size: 1.875em;
  }
</style>
