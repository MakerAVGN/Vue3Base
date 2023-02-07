<script>
export default {
  data() {
    return {
      text: 'like',
    }
  },
  methods: {
    change: function () {
      this.text = 'hate';
    },
    change1: function () {
      this.text = 'eat';
    }
  }
  
}


</script>
<template>
<h1>№1</h1> <br>
<p>I {{ text }} pumpkin</p>
<button @click="change" >switch</button>
<button @click="change1">switch2</button>
</template>