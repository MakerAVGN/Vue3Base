<script>
export default {
  data() {
    return {
      number: 1,
      number_square: "Task 1",
      number1: 0,
      number2: 0,
      sum_number: "Task 2",
      text1: "placeholder",
      text2: "placeholder",
      fullName: "",
      userName: "",
      userSurname: "",
      userPatronymic: "",
    };
  },
  methods: {
    square: function () {
      this.number_square = this.number ** 2;
    },
    sum: function () {
      this.sum_number = this.number1 + this.number2;
    },  
    swap: function () {
      const temp = this.text1;
      this.text1 = this.text2;
      this.text2 = temp;
    },
  },
};
</script>
<template>
    <input type="number" v-model="number" />
    <button @click="square">Square of number</button>
    <br>
    <p>{{ number_square }}</p>
    <br>
    
    <input type="number" v-model="number1" />
    <input type="number" v-model="number2" />
    <button @click="sum">Summ of numbers</button>
    <br>
    
    <p>{{ sum_number }}</p>
    <br>
    
    <input type="text" v-model="text1" />
    <input type="text" v-model="text2" />
    <button @click="swap">Swap values</button>
    <br>
    
</template>
<style>

</style>


