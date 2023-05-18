<script>
export default {
 data() {
    return {
      selected: 'Симферополь', // значение по умолчанию
    }
  },
  methods: {},
};
</script>
<template>
  <p>В каком городе вы живете?</p>
 	<select v-model="selected">
  		<option>Симферополь</option>
  		<option>Севастополь</option>
  		<option>Керчь</option>
  	</select>
	
  	<p>{{ selected }}</p>




</template> 
<style>

</style>


