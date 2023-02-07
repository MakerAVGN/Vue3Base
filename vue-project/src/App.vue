<script>
export default {
  data() {
    return {
      text:'Модификаторы событий в фреймворке Vue',
      url: 'https://v3.ru.vuejs.org/ru/guide/events.html#модификаторы-событии'
    }
  },
  methods: {
    warning: function(){
      alert('JUST ONE TIME!');
    }
  }
}
</script>
<template>
  <a @click.prevent :href=url>{{ text }}</a> <br>
  <button @click.once="warning"> Just one time </button>
</template>
