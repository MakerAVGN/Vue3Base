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
  <p :class="{ active: isActive, error: hasError }">
    text
  </p>
</template>

<style>
.active {
  border: 10px solid black;
}
.error   {
  color: red;
}
</style>


