<script>
import User from './components/User.vue'
import Employee from './components/Employee.vue'

export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'name1',
          surn: 'surn1'
        },
        {
          id: 2,
          name: 'name2',
          surn: 'surn2'
        },
        {
          id: 3,
          name: 'name3',
          surn: 'surn3'
        },
      ],
    }
  },
  components: {
    User,
    Employee
  },
 methods: {
    add(name, surn) {
      let id = this.users.length + 1;

      this.users.push({
        id,
        name,
        surn
      });
    }
  },
};
</script>
<template>

 		<User @add="add" />

    {{ users }}

</template>
<style>

</style>


