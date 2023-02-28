<script>
export default {
  data() {
    return {
      obj: {
        done: true,
        selected: false,
      },
    }
  }
}
</script>
<template>
  <p :class="obj">text</p>
</template>



