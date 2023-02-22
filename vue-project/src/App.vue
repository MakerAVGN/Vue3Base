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
 <button class="a" @click="add" >Task1</button>
  <button class="a"  @click="delFirst" >Task2</button>
  <button class="a"  @click="delLast" >Task3</button>
  <button class="a"  @click="delSecondLast" >Task4</button>
  <button class="a"  @click="sortarr" >Task5</button>
  <button class="a"  @click="reverseMassive" >Task6</button>

  <ul class="b"  v-for="elem in arr">
      <li>{{ elem }}</li>
    </ul><br>
</template>



