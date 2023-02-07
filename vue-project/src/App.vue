<script>
export default {
  data() {
    return {
      text: 'str',
      num1: 1,
      num2: 2,
    }
  },
  methods: {
    summ: function () {
      const number = this.$refs.inputmult.value;
      alert(number * number);
    },

    mult_two: function() {
      alert(2 * 2);
    },
    mult_three: function () {
      alert(3 * 3);
    }
  }
  
}


</script>
<template>
<h1>№1</h1> <br>
<input type="number" ref="inputmult"><br>
<button @click="summ">Click</button>
<br>
<br>


<button @click="mult_two">Square number 2</button> <br>
<button @click="mult_three">Square number 3</button>
</template>