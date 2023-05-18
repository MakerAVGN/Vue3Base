<script>
export default {
  data() {
    return {
      newItem: '',
      items: ['a', 'b', 'c', 'd', 'e'],
    }
  },
  methods: {
   removeItem: function (index) {
      this.items.splice(index, 1);
    }
  },
};
</script>
<template>

  <ul>
  		<li v-for="(item, index) in items" :key="index">
  			{{ item }} 
        <button @click="removeItem(index)">remove</button>
  		</li>
      
  	</ul>

  <input v-model="newItem">
  	<button @click="addItem">add</button>





</template> 
<style>

</style>


