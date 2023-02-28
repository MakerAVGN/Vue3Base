<script>
export default {
  data() {
    return {
      obj: {
        hidden: true,
      },
    }
  },
  methods: {
    setfalse: function () {
      this.obj.hidden = false;
    },
    settrue: function () {
      this.obj.hidden = true;
    },
    setDone: function () {
      this.obj.hidden = !this.obj.hidden;
  }
}
}
</script>
<template>
  <p :class="obj">text</p>
  	<button @click="settrue">hide</button> <br>
    <button @click="setfalse">show</button><br>
      <button @click="setDone">{{ obj.hidden ? "show" : "hide" }}№4</button><br />
</template>

<style>
p.hidden {
	display: none;
}
</style>


