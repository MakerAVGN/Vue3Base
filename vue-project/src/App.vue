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
      name: 'john',
      surn: 'smit',
      age: '15'
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

<Employee :name="name" :surn="surn" :age="age" />

  <Employee />





</template>
<style>

</style>


