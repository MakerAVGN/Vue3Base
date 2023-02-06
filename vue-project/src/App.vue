<script>
export default {
  data() {
    return {
      text:'Cute kitty video',
      href: 'https://www.youtube.com/watch?v=xosMyvzRoPM'
    }
  }
}
</script>
<template>
<a :href=href>{{ text }}</a>
</template>