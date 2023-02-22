<script>
export default {
  data() {
    return {
      visible: true,
    }
  },
  methods: {
    toggle: function () {
      this.visible = !this.visible;
    }
    
  }
}
</script>
<template>
  <button @click="toggle">toggle</button>
  <p v-if="visible">text</p>
</template>
