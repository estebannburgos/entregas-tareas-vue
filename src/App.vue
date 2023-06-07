<template>
  <div>
    <HelloWorld :data="data1" bg-color="lightblue" text-color="black" />
    <HelloWorld :data="data2" bg-color="lightgreen" text-color="white" />
    <HelloWorld :data="data3" bg-color="lightyellow" text-color="black" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  components: {
    HelloWorld
  },
  data() {
    return {
      data1: [
        { id: 1, nombre: 'Pedro', edad: 25 },
        { id: 2, nombre: 'Juan', edad: 30 },
        { id: 3, nombre: 'Diego', edad: 35 }
      ],
      data2: [
        { id: 4, nombre: 'María', edad: 28 },
        { id: 5, nombre: 'Luisa', edad: 32 },
        { id: 6, nombre: 'Camila', edad: 40 }
      ],
      data3: [
        { id: 7, nombre: 'Marcelo', edad: 27 },
        { id: 8, nombre: 'Daniela', edad: 31 },
        { id: 9, nombre: 'Miguel', edad: 38 }
      ]
    };
  }
}
</script>

<style>

body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    margin: 0;
    padding: 20px;
  }
  
  h1 {
    color: #333;
    font-size: 24px;
    font-weight: bold;
  }
  
  p {
    color: #666;
  }

  .fila-par {
    background-color: #f2f2f2;
  }

  .fila-impar {
    background-color: #ffffff;
  }
  
  h2 {
    font-size: 20px;
    font-weight: bold;
  }
  
  h3 {
    font-size: 18px;
    font-weight: bold;
  }
  
  h4 {
    font-size: 16px;
    font-weight: bold;
  }
  
  h5 {
    font-size: 14px;
    font-weight: bold;
  }
  
  h6 {
    font-size: 12px;
    font-weight: bold;
  }
</style>
