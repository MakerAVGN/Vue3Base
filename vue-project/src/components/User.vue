<script>
export default {
    emits: ['show'],
    data() {
        return {
        }
    },
    methods: {
        handle() {
            this.$emit('show','muhammed', 123);
            
        }
    }
}
</script>
<template>
    <button @click="handle">btn</button>
</template>