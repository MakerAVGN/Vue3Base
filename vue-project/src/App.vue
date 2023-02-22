<script>
export default {
 data() {
    return {
      arr: ['a', 'b', 'c'],
    }
  },
  methods: {
    add: function () {
      this.arr.push('xxx');
    },
    delFirst: function(){
        this.arr.shift();
    },
    delLast: function() {
      this.arr.pop();
    },
    delSecondLast: function() {
      this.arr.splice(-2,1);
    },
    sortarr: function(){
      this.arr.sort();
    },
    reverseMassive: function(){
      this.arr.reverse();
    }
  }

}
</script>
<template>
<p class="a">Я уже стилизирован</p>
<p class="b"> А я тем более</p>
</template>



