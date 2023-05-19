<script>
import User from './components/User.vue'
import Employee from './components/Employee.vue'

export default {
  components: {
    User,
    Employee
  },
  data() {
    return {
      
    }
  },
 methods: {
    edit(user) {
      user.isEdit = true;
    },
    save(user) {
      user.isEdit = false;
    }
  },
};
</script>
<template>
  
  <User /> <Employee />





</template>
<style>

</style>


