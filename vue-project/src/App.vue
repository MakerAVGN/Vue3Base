<script>
import User from './components/User.vue'
import Employee from './components/Employee.vue'

export default {
 data() {
    return {
      users: [
        {
          id: 1,
          name: 'Учеба',
          surn: 'Сделать домашку по аипу'
        },
        {
          id: 2,
          name: 'Готовка',
          surn: 'Приготовить себе спагетти'
        },
        {
          id: 3,
          name: 'Уборка',
          surn: 'Прибраться в своей комнате'
        },
      ],
    }
  },
  components: {
      User,
      Employee
  },
 methods: {
  change(id, name, surn) {
      this.users = this.users.map((user) => {
        if (user.id === id) {
          user.name = name;
          user.surn = surn;
        }
        return user;
      });
    },
    remove(id) {
      this.users = this.users.filter((user) => {
        return user.id !== id;  
      })
    },
    add(name, surn) {
      let id = this.users.length + 1;

      this.users.push({
        id,
        name,
        surn
      });
    },
  },
};
</script>
<template>

 <User
  		v-for   ="user in users"
		
  		:id     ="user.id"
  		:name   ="user.name"
  		:surn   ="user.surn"
  		@remove ="remove"
      @change="change"
      @add="add"
  		:key    ="user.id"
  	/>

</template>
<style>
ul.done {
  text-decoration: line-through;
}
</style>


