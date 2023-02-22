<script>
export default {
  data() {
    return {
          isAuth: true,         
    }
  },
  methods: {
    toggle: function () {
      this.visible = !this.visible;
    },
    toggle1: function () {
      this.visible1 = !this.visible1;
    },
    toggle2: function () {
      this.visible2 = !this.visible2;
    }
    
  }
}
</script>
<template>
  <p v-if="isAuth">+++</p>
  <p v-else>---</p>
</template>