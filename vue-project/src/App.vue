<script>
export default {
  data() {
    return {
      visible: true,
      not_visible: false,
    }
  },
  methods: {
    
    
  }
}
</script>
<template>
  <p v-if="visible" > Видишь меня? </p>
  <p v-if="not_visible" > А меня нет))) </p>
</template>
