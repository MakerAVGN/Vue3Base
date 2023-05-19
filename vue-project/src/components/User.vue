<script>
export default {
    data() {
        return {
            newName: '',
            newSurn: '',
        }
    },
    props: {
        id: Number,
        name: String,
        surn: String,
    },
    emits: ['add'],
    methods: {
        save() {
            this.$emit('add', this.newName, this.newSurn);
        }
    }
}
</script>
<template>

        <input v-model="newName">
    	<input v-model="newSurn">
	
    	<button @click="save">
    		save
        </button>
        

</template>