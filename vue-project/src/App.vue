<script>
export default {
 data() {
    return {
      isActive: true,
      hasError: true,
    }
  },
  methods: {
    
}
}
</script>
<template>
  <p :style="{ color: 'green', 'background-color': 'yellow' }">
    text
  </p>
  <p :style="{'font-weight': 800, 'font-style': 'italic'}">
    text 2
  </p>
</template>

<style>

</style>


