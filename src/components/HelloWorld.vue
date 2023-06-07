<template>
  <table :style="{ backgroundColor: bgColor, color: textColor }">
    <tr>
      <th>Nombre</th>
      <th>Edad</th>
    </tr>
    <tr v-for="item in data" :key="item.id">
      <td>{{ item.nombre }}</td>
      <td>{{ item.edad }}</td>
    </tr>
  </table>
</template>

<script>
export default {
  props: {
    data: {
      type: Array,
      required: true
    },
    bgColor: {
      type: String,
      default: 'white'
    },
    textColor: {
      type: String,
      default: 'black'
    }
  }
}
</script>

<style scoped>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  border: 1px solid black;
  padding: 8px;
}
</style>
