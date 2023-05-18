<script>
export default {
  data() {
    return {
      isDisabled: false,
    }
  },
  methods: {
    a: function () {
      this.isDisabled = !this.isDisabled
    }
  },
};
</script>
<template>


  	<input :disabled="isDisabled" >

    <input type="checkbox" v-model="isDisabled">







</template> 
<style>

</style>


