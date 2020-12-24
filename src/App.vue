<template>
  <div id="app">
    <HelloWorld v-bind:value="info">
        <h2>С новым годом!</h2>
    </HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return{
      info: {
        name: "Новогодняя пицца",
        price: "599руб",
        size: "40см",
        include: "тесто, сыр, кетчеп, колбаса, томаты",
        img: "https://static.pizzasushiwok.ru/images/menu_new/6-1300.jpg"
      }
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h2 {
  font-size: 20px;
  font-family: 'Courier New', Courier, monospace;
  color: crimson;  
}
</style>
