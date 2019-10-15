<template>
  <button :class="active ? 'btn' : 'btn-disabled'">
    <span>{{text}}</span>
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    active: Boolean
  },
  computed: {
    btnClass() {
      return this.active ? 'active' : 'disabled';
    }
  },
  mount() {

  }
}

</script>

<style lang="css" scoped>
  .btn, .btn-disabled {
    text-transform: uppercase;
    border-width: 3px;
    border-color: rgb(93, 93, 93);
    border-style: solid;
    background-color: #99cc33;
    line-height: 38px;
    font-weight: 300;
    color: #ffffff;
    font-size: 1.875em;
    font-weight: 300;
    padding: 0px 10px;
    cursor: pointer;
    position: relative;
    overflow: hidden;
  }
  .btn-disabled {
    background-color: #999;
  }
  .btn::before,
  .btn::after {
    content: attr(data-text);
    position: absolute;
    width: 100%;
    height: 50%;
    left: 0;
    right: 0;
    background: rgb(101, 156, 193);
    color: #fff;
    overflow: hidden;
    -webkit-transition: -webkit-transform 0.3s;
    transition: transform 0.3s;
    -webkit-transition-timing-function: cubic-bezier(0.2, 1, 0.3, 1);
    transition-timing-function: cubic-bezier(0.2, 1, 0.3, 1);
  }
  .btn::before {
    top: -0.3px;
    /*padding-top: 1em;*/
  }
  .btn::after {
    bottom: -0.3px;
    line-height: 0;
  }
  .btn > span {
    display: block;
    -webkit-transform: scale3d(0.2, 0.2, 1);
    transform: scale3d(0.2, 0.2, 1);
    opacity: 0;
    -webkit-transition: -webkit-transform 0.3s, opacity 0.3s;
    transition: transform 0.3s, opacity 0.3s;
    -webkit-transition-timing-function: cubic-bezier(0.2, 1, 0.3, 1);
    transition-timing-function: cubic-bezier(0.2, 1, 0.3, 1);
  }
  .btn:hover::before {
    -webkit-transform: translate3d(0, -100%, 0);
    transform: translate3d(0, -100%, 0);
  }
  .btn:hover::after {
    -webkit-transform: translate3d(0, 100%, 0);
    transform: translate3d(0, 100%, 0);
  }
  .btn:hover > span {
    opacity: 1;
    -webkit-transform: scale3d(1, 1, 1);
    transform: scale3d(1, 1, 1);
  }
</style>
