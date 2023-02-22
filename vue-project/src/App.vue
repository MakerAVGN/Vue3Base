<script>
export default {
  data() {
    return {
      
        items: [1, 2, 3],
      
    }
  },
  methods: {
  }
}
</script>
<template>
 <template v-for="elem in arr">
		<p>{{ elem }}</p>
		<hr>
	</template>
  	
    <li class="a" v-for="elem in items">
        <ul>
         {{ elem }}
        </ul>
      </li>
      <br>

</template>



