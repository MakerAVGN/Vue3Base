<script>
export default {
  data() {
    return {
      obj: { x: 1, y: 2, z: 3 },
    }
  }
}
</script>
<template>
<h1>№1</h1> <br>
<h2>{{ obj['x'] + obj['y'] + obj['z'] }}</h2>

</template>