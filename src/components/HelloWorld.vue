<template>
  <div>
    <h1>{{value.name}}</h1>
    <p class="price">Цена - {{value.price}}</p>
    <p class="size">Размер - {{value.size}}</p>
    <p class="include">Состав - {{value.include}}</p>
    <img v-bind:src="value.img">
    <slot />
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: ['value']
}
</script>

<style scoped>
h1{
  font-size: 30px;
  font-family: 'Courier New', Courier, monospace;
  color: crimson;
}

p{
  font-size: 20px;
  font-family: 'Courier New', Courier, monospace;
  color: brown;
}

.include {
  font-size: 18px;
}
img {
  width: 500px;
  height: 500px;
}
</style>
