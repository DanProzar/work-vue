<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
import Header from './components/Header'
export default {
  name: 'App',
  components: {
    Header
  }
};
</script>
<style lang="scss">
  @font-face {
  font-family: 'PFDinTextCondPro';
  src: url('./assets/fonts/Light/PFDinTextCondPro-Light.eot?#iefix') format('embedded-opentype'),  url('./assets/fonts/Light/PFDinTextCondPro-Light.woff') format('woff'), url('./assets/fonts/Light/PFDinTextCondPro-Light.ttf')  format('truetype'), url('./assets/fonts/Light/PFDinTextCondPro-Light.svg#PFDinTextCondPro-Light') format('svg');
  font-weight: 300;
  font-style: normal;
}
@font-face {
  font-family: 'PFDinTextCondPro';
  src: url('./assets/fonts/Medium/PFDinTextCondPro-Medium.eot?#iefix') format('embedded-opentype'),  url('./assets/fonts/Medium/PFDinTextCondPro-Medium.woff') format('woff'), url('./assets/fonts/Medium/PFDinTextCondPro-Medium.ttf')  format('truetype'), url('./assets/fonts/Medium/PFDinTextCondPro-Medium.svg#PFDinTextCondPro-Medium') format('svg');
  font-weight: 500;
  font-style: normal;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'PFDinTextCondPro' !important;
}
.d-flex {
  display: flex;
  align-items: center;
  justify-content: center;
}
body {
  font-size: 16px;
  line-height: 1.2;

  .container{
    padding: 0 46px;
  }
}
.t-right {
  text-align: right;
}


</style>
