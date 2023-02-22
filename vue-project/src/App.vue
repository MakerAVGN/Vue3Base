<script>
export default {
 data() {
    return {
      products: [
        {
          id: 1,
          name: 'product1',
        },
        {
          id: 2,
          name: 'product2',
        },
        {
          id: 3,
          name: 'product3',
        },
      ]
    }
  }
}
</script>
<template>
<ul>
    <li v-for="user in products" :key="user.id">
      {{ user.name }}
    </li>
  </ul>
</template>



