<script>
export default {
  data() {
    return {
      items: [1, -2, 3, -4, 5],
    }
  },
  methods: {
  }
}
</script>
<template>
	<ul>
		<template v-for="elem in items">
			<li v-if="elem > 0">
				{{ elem }}
			</li>
		</template>
	</ul>
</template>



