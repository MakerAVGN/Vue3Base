<script>
export default {
    emits: ['show','aboba'],
    props: {
        name: String,
        surn: String,

    },
    data() {
        return {

        }
    },
    methods: {
        handle() {
            this.$emit('show');
        },
        aboba() {
            this.$emit('aboba')
        }
    }
}
</script>
<template>


        
    <button @click="handle">btn</button>
    <button @click="aboba">aboba</button>
  

    	

</template>