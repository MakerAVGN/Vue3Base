<script>
export default {
  data() {
    return {
      text: "",
      text_button: "",
      text_array: "",
    };
  },
  methods: {
    split_text: function () {
      this.text_array = this.text_button.split(" ");
    },
  },
};
</script>
<template>
  <textarea v-model="text"></textarea>
  &nbsp;
  <p>{{ text }}</p>
  &nbsp;
  <textarea v-model="text_button"></textarea>
  &nbsp;
  <button @click="split_text">Array</button>
  &nbsp;
  <ul v-for="elem in text_array">
    <li :key="key">
      {{ elem }}
    </li>
  </ul>
</template>
<style>

</style>


