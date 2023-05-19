<script>
export default {
    props: {
        id: Number,
        name: String,
        surn: String,
    },
    emits: ['remove'],
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
    	{{ name }}
    	{{ surn }}
        <button @click="$emit('remove', id)">
    		remove
    	</button>
</template>