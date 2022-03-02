<template>
  <div id="app">
    <HeaderComp />
    <CardComp />
    <AboutComp />
    <FooterComp />
  </div>
</template>

<script>
import CardComp from './sections/Card.vue'
import HeaderComp from './sections/Header.vue'
import AboutComp from './sections/About.vue'
import FooterComp from './sections/Footer.vue'

const components = {
  HeaderComp,
  CardComp,
  AboutComp,
  FooterComp,
}

export default {
  name: 'App',
  components
}
</script>

<style lang="scss">
$green: #00ffbb;
$bg-color: #212121;

* {
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  list-style: none;
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  background-color: $bg-color;
}
</style>