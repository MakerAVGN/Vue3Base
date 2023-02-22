<script>
export default {
  data() {
    return {
          age: 2,  
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
  <p v-if="age < 18"> Подросток</p>
  <p v-else-if="age <= 25"> Молодой человек</p>
  <p v-else-if="age >= 26"> Мужчина</p>
</template>