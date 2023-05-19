<script>
import User from './components/User.vue'
import Employee from './components/Employee.vue'

export default {
  components: {
    User,
    Employee
  },
  methods: {
    func(arg1, arg2) {
      console.log(arg1, arg2);
    },
    handle() {
      this.$emit('show', 'xxx', 'yyy');
    },
  },
};
</script>
<template>

 <div>
        <button @click="handle">Нажми меня</button>
        <User @show="func"/>
      </div>



</template>
<style>

</style>


