<script>
export default {
    data() {
        return {
            isEdit: false,
            editName: this.name,
            editSurn: this.surn,
            newName: '',
            newSurn: '',
            styles: {
                done: false,
            },
        }
    },
   props: {
        id: Number,
        name: String,
        surn: String,
    },
    emits: ['show'],
    methods: {
        edit() {
            this.isEdit = true;
        },
        save() {
            this.isEdit = false;
            this.$emit('change', this.id, this.editName, this.editSurn);
        },
        saveNewElement() {
            this.$emit('add', this.newName, this.newSurn);
        },
        setDone: function () {
            this.styles.done = true;
        }
    }
}
</script>
<template>
     <ul :class="{ 'done': styles.done }">
    	<template v-if="!isEdit" >
            <button @click="setDone">Выполнил</button>
    		{{ name }}
    		{{ surn }}
    		<button @click="edit">
    			Изменить
    		</button>
            <button @click="$emit('remove', id)">
        		Удалить
        	</button>
    	</template>
    	<template v-else>
    		<input v-model="editName">
    		<input v-model="editSurn">
    		<button @click="save">
    			save
    		</button>
    	</template>
        </ul>

    <div style="margin-left: 50px;">
            <p>Новая задача</p>
            <input v-model="newName">
        	<input v-model="newSurn">
	
        	<button @click="saveNewElement">
        		Сохранить
        	</button>
    </div>
</template>


<style>
ul  .done {
	text-decoration: line-through;
}
</style>