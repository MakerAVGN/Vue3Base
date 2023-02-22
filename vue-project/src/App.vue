<style>
div {
  display: flex;
  font-size: 1.2rem;
}
.a{
  border: 3px solid purple;
  margin: 5px;
  padding: 5px;
  align-items: center;
}
.b{
  border: 3px solid yellow;
  flex-direction: column;
  text-align: center;
  margin: 5px;
}
</style>
<script>
export default {
  data() {
    return {
      items: [1, 2, 3, 4, 5],
      items1: [1, 2, 3, 4, 5],
      items2: [1, 2, 3, 4, 5],
    }
  },
  methods: {
    toggle: function () {
      this.isAuth = !this.isAuth;
    }
    
  }
}
</script>
<template>
  <p v-for="elem in items" class="b">{{ elem }}</p>
  <br>
  <br>
  <div class="a">
  <p v-for="amo in items1">{{ amo*amo }};</p>
  </div>
  <br>
  <br>
  <br>
  <br>
  <br>
<p v-for="go in items2" class="b" ><ul><li>{{ go }}</li></ul></p>

</template>



