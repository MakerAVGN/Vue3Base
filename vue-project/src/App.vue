<script>
export default {
  data() {
    return {
      num: 0,
    }
  },
  methods: {
  }
}
</script>
<template>
  <p v-for="num in 30" style="padding: 5px;">
    {{ num }}
  </p>
</template>



