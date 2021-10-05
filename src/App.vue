<template>
  <div id="app">
    <Header />
    <Promo />
    <About />
    <Configurator />
    </div> 
</template>

<script>
import Header from './components/Header.vue'
import Promo from './components/Promo.vue'
import About from './components/About.vue'
import Configurator from './components/Сonfigurator.vue'

export default {
  name: 'App',
  components: {
    Header, Promo, About, Configurator
  }
}
</script>

<style>

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

@font-face {
  font-family: 'Rosanthie';
  src: local('Rosanthie'), 
    url('./assets/fonts/Rosanthie.woff') format('woff');
  font-style: normal;
  font-weight: 400;
}

@font-face {
  font-family: 'Kudryashev Display';
  src: local('Kudryashev Display') 
    url('./assets/fonts/KudryashevDisplaySans.woff2') format('woff2');
    font-style: normal;
    font-weight: normal;
    
}

body {
  background: #ffffff;
  margin: 0;
  padding: 0;
  font-family: 'Geometria';
  color: #000000;
  font-size: 14px;
  font-weight: 300;
  line-height: 24px;
}

.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 165px;
}

.title {
  font-family: 'Kudryashev Display';
  font-weight: 400;
  font-size: 40px;
  line-height: 50px;
}

.button {
  display: block;
  width: 230px;
  padding: 12px 30px;
  border: 3px solid #000000;
  box-sizing: border-box;
  background: #ffffff;
  font-family: "Geometria";
  text-transform: uppercase;
  line-height: 20px;
  font-weight: 700;
}

.Rosanthie-text {
  font-family: 'Rosanthie';
  font-size: 154px;
  line-height: 154px; 
  color: #EDEDED;
  transform: rotate(-17.46deg);
  position: absolute;
  font-weight: 400;
}

a {
    text-decoration: none;
    color: #000000;
    cursor: pointer;
}

ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

.gray {
    color: #A3A3A3;
}

</style>
