<script>
export default {
  data() {
    return {
      arr: ['x', 'y', 'z'],
      arr: [1, 2, 3],
    }
  }
}
</script>
<template>
<p>№1</p> <br>
<h1>{{ arr[0] }}</h1> <br>
<h2>{{ arr[1] }}</h2><br>
<h3>{{ arr[2] }}</h3> <br> <br>
<p>№2</p> <br>

<p>{{ arr[0] + arr[1] + arr[2] }}</p>

</template>