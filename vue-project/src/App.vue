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
    show: function () {
      alert(this.num1 + this.num2);
    }
  }
}
</script>
<template>
<h1>№2</h1> <br>
<button @click="show">Date</button>


</template>