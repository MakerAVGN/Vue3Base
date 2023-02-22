<style>
*{
  background-color: #3d405b;
}
div {
  display: flex;
  font-size: 1.2rem;
}
.a{
  border: 3px solid #e07a5f;
  margin: 5px;
  padding: 10px;
  align-items: center;
  flex-direction: column;
  color:#e07a5f ;
}
.b{
  border: 3px solid #f4f1de;
  flex-direction: column;
  text-align: center;
  margin: 5px;
  padding: 10px;
  color: #f4f1de;
}
</style>
<script>
export default {
  data() {
    return {
        arr: ['x', 'y', 'z'],
    }
  },
  methods: {
    toggle: function () {
      this.isAuth = !this.isAuth;
    }
    
  }
}
</script>
<template>
 <p class="b" v-for="(elem, key) in arr">
  		 <ul><li>{{ key + 1 }} {{ elem }}</li></ul>
  	</p>

  <p class="a" v-for="(elem, key) in arr">
    		 <ul><li>{{ key + 1 }} {{ elem }}</li></ul>
    	</p>
</template>



