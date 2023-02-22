<script>
export default {
  data() {
    return {
         isAuth: true, 
    }
  },
  methods: {
    toggle: function () {
      this.isAuth = !this.isAuth;
    }
    
  }
}
</script>
<template>
   <button @click="toggle">Кнопка</button>
   <br>
  <div v-if="isAuth">
    <p>+++</p>
    <p>+++</p>
    <p>+++</p>
  </div>
</template>