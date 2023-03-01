<script>
export default {
 data() {
    return {
      choice: '',
    }
  },
  methods: {},
};
</script>
<template>
  <input name="radio" type="radio" v-model="choice" value="Russian">
  <br>
  <p>Russian</p><br>
  <input name="radio" type="radio" v-model="choice" value="English"><br>
  <p>English</p><br>
  <input name="radio" type="radio" v-model="choice" value="Tatar"><br>
  <p>Tatar</p><br>
  <p>{{ choice }}</p>
</template> 
<style>

</style>


