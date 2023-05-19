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


  <User :arg="[1, 2, 3]" />
 <User :arg="{ a: 1, b: 2, c: 3 }" />
 	<User :arg="true" />

  <User />





</template>
<style>

</style>


