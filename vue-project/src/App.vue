<script>
export default {
  data() {
    return {
          day: 3,      
    }
  },
  methods: {
    toggle: function () {
      this.visible = !this.visible;
    },
    toggle1: function () {
      this.visible1 = !this.visible1;
    },
    toggle2: function () {
      this.visible2 = !this.visible2;
    }
    
  }
}
</script>
<template>
  <p >Today: </p>
  <p v-if="day == 1">Monday</p>
  <p v-if="day == 2">Tuesday</p>
  <p v-if="day == 3">Wednesday</p>
  <p v-if="day == 4">Thursday</p>
  <p v-if="day == 5">Friday</p>
  <p v-if="day == 6">Saturday</p>
  <p v-if="day == 7">Sunday</p>
</template>