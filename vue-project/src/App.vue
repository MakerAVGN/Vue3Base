<script>
export default {
  data() {
    return {
      visible: true,
    }
  },
  methods: {
    hide: function() {
      this.visible = false;
    },
    show: function () {
      this.visible = true;
    },
    
  }
}
</script>
<template>
<button v-if="visible" @click="hide">Hide text</button>
<p v-if="visible"> HELLO! </p>
<button v-if="!visible" @click="show">Show text</button>

</template>
