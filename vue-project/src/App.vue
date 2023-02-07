<script>
export default {
  data() {
    return {
      cost: 5,
      amount: 10,
    }
  },
  computed: {
    summ: function () {
      return this.amount * this.cost;
    },
    izm: function () {
      this.cost = this.cost + 3;
    }
 
  }
  
}


</script>
<template>
<h1>№1</h1> <br>
  <p>{{ cost }}</p>
  <p>{{ amount }}</p>
  <p>{{ summ}}</p>
  <button @click="izm" >+3 cost</button>
</template>