<script>
export default {
  data() {
    return {
      newItem: '',
      items: ['a', 'b', 'c', 'd', 'e'],
    }
  },
  methods: {
   addItem() {
    this.items.unshift(this.newItem);
   }
  },
};
</script>
<template>

  <ul>
  		<li v-for="(item, index) in items" :key="index">
  			{{ item }} 
  		</li>
  	</ul>

  <input v-model="newItem">
  	<button @click="addItem">add</button>





</template> 
<style>

</style>


