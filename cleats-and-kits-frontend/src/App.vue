<template>
  <div id="app">
    <Header />
    <Bodyy />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Bodyy from './components/Bodyy.vue'
export default {
   name: 'App',
  components: {
    Header,
    Bodyy
  }
}
</script>

<style>
 
#app {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-image: linear-gradient(pink, white, white, white);
}
 /*  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}*/
</style>