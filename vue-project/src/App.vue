<script>
export default {
  data() {
    return {
      data: {
        user1: '100$',
        user2: '200$',
        user3: '300$',
      }
    }
  },
  methods: {
  }
}
</script>
<template>
  	<div class="a">
      <p v-for="elem in data">
      {{ elem }}; </p>
    </div>

    <div class="b">
      <p v-for="(elem,key) in data" >
      {{ key }} - {{ elem }}</p>
    </div>

    <div class="b">
      <p v-for="(elem,key, index) in data" >
      {{ key }} - {{ elem }} - {{ index }}</p>
    </div>
    <div class="a">
        <p v-for="(elem, key, index) in data" >
        {{ key }} - {{ elem }} - {{ index + 1 }}</p>
      </div>
</template>



