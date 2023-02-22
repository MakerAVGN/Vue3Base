<script>
export default {
  data() {
    return {
      visible: true,
      visible1: true,
      visible2: true
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
  
  	<button @click="toggle">{{ visible ? 'hide' : 'show' }}</button>
    <button @click="toggle1">{{ visible1 ? 'hide' : 'show' }}</button>
    <button @click="toggle2">{{ visible2 ? 'hide' : 'show' }}</button>
</template>
