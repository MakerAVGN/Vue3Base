<script>
import User from './components/User.vue'
import Employee from './components/Employee.vue'

export default {
  components: {
    User,
    Employee
  },
  methods: {
    func(name, salary) {
      console.log(name, salary);
    }
  },
};
</script>
<template>


        
        <User @show="func"/>
 



</template>
<style>

</style>


