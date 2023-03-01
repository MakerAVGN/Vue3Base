<script>
export default {
  data() {
    return {
      task: "Task",
      number: 3,
    }
  },
  methods: {
    
}
}
</script>
<template>
 <input type="text" v-model="task" /><br>
  <p>{{ task }}</p><br>
  <p>{{ task.toUpperCase() }}</p><br>
  <input type="number" v-model="number" /><br>
  <p>{{ number ** 2 }}</p><br>
</template>

<style>

</style>


