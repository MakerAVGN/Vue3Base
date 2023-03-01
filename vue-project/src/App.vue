<script>
export default {
  data() {
    return {
      checked: true,
    };
  },
  methods: {},
};
</script>
<template>
  <input type="checkbox" v-model="checked" />
  &nbsp;
  <p v-if="checked">{{ checked }}</p>
</template>
<style>

</style>


