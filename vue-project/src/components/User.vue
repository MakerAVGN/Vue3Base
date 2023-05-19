<script>
export default {
    emits: ['show'],
    data() {
        return {
        }
    },
    methods: {
        handle() {
            const a = this.$emit('kokiev', 'muhammed', '123');
            console.log(a);
        }
    }
}
</script>
<template>
    
</template>