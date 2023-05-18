<script>
export default {
  data() {
    return {
      inputText: "",
      displayedText: "",
      task_2: false,
      task_3: '',
      outputText: ''
    }
  },
  methods: {
    displayText() {
      this.displayedText = this.inputText;
    },
    text1() {
      this.task_2 = true;
    },
    left() {
      this.outputText = 'left'
    },
    right() {
      this.outputText = 'right'
    },
    middle() {
      this.outputText = 'middle'
    }
  },
};
</script>
<template>


 <div >
      <input type="text" v-model="inputText" @keydown.enter="displayText" />
      <p>{{ displayedText }}</p>
    </div>


    <a href="/" @click.ctrl="text1">Ссылка</a>
    <p v-if="task_2">asdasds</p>


    <a href="/" @click.left.prevent="left" @click.right.prevent="right"  @click.middle.prevent="middle">Ссылка 2</a>
     <p>{{ outputText }}</p>






</template> 
<style>

</style>


