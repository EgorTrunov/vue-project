<template>
  <div id="app">
    <Header />
    </div> 
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>
body {
  background: #f5f5f5;
  margin: 0;
  padding: 0;
}

.container {
  width: 1100px;
  margin: 0 auto;
  padding: 35px 165px;
}

@font-face {
  font-family: 'Geometria';
  src: local('Geometria Bold'),
    url('./assets/fonts/Geometria-Bold.woff') format('woff');
  font-weight: 700;
  font-style: normal;
}

@font-face {
  font-family: 'Geometria';
  src: local('Geometria Medium'),
    url('./assets/fonts/Geometria-Medium.woff') format('woff');
  font-weight: 500;
  font-style: normal;
}

@font-face {
  font-family: 'Geometria';
  src: local('Geometria Regular'),
    url('./assets/fonts/Geometria-Regular.woff') format('woff');
  font-weight: 400;
  font-style: normal;
}

@font-face {
  font-family: 'TT Norms Pro';
  src: local('TT Norms Pro Regular'),
    url('./assets/fonts/TTNormsPro-Regular.woff') format('woff');
  font-weight: 400;
  font-style: normal;
}

@font-face {
  font-family: 'TT Norms Pro';
  src: local('TT Norms Pro Medium'),
    url('./assets/fonts/TTNormsPro-Medium.woff') format('woff');
  font-weight: 500;
  font-style: normal;
}
.button {
  width: 230px;
  padding: 12px 30px;
  border: 3px solid #000000;
  box-sizing: border-box;
  background: #f5f5f5;
  font-family: "Geometria";
  text-transform: uppercase;
  line-height: 20px;
  font-weight: 700;
}
</style>
