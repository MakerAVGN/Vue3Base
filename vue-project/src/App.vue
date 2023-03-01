<script>
export default {
 data() {
    return {
      arr: [],
    }
  },
  methods: {},
};
</script>
<template>
  <input type="checkbox" v-model="arr" value="english"><br>
  <p>English</p><br>
  <input type="checkbox" v-model="arr" value="russian"><br>
   <p>Russian</p><br>
  <input type="checkbox" v-model="arr" value="japan"><br>
   <p>Japan</p><br>
  <ul v-for="elem in arr"> 
    <li>
      {{ elem }}
    </li>
  </ul>
</template>
<style>

</style>


