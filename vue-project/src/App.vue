<script>
export default {
  data() {
    return {
      day: 'Понедельник',
      days: ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье'],
      month: 'Январь',
      months: ['Январь', 'Февраль'],
      year: '2000',
      years: ['2000', '2001']
    }
  },
  methods: {},
};
</script>
<template>
  <div>
 <select v-model="day">
  		<option v-for="day in days">{{ day }}</option>
  	</select>
  	<p>{{ selected }}</p>
  </div>

  <div>
    <select v-model="month">
    		<option v-for="month in months">{{ month }}</option>
    	</select>
    	<p>{{ selected }}</p>
  </div>

  <div>
      <select v-model="year">
      		<option v-for="year in years">{{ year }}</option>
      	</select>
      	<p>{{ selected }}</p>
    </div>







</template> 
<style>

</style>


