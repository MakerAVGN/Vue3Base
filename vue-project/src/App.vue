<template>
  <div>
    <div class="sidebar">
      <input class="search" type="text" v-model="searchText" placeholder="Search...">
      <ul>
        <li v-for="note in filteredNotes" :key="note.id" @click="selectNote(note)">
          {{ note.title }}
          <button @click.stop="deleteNote(note)">Delete</button>
        </li>
      </ul>
    </div>
    <div class="content">
      <textarea v-model="currentNote.content"></textarea>
      <button @click="editMode = !editMode">{{ editMode ? 'Save' : 'Edit' }}</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      notes: [
        { id: 1, title: 'Note 1', content: 'Content of note 1' },
        { id: 2, title: 'Note 2', content: 'Content of note 2' },
        { id: 3, title: 'Note 3', content: 'Content of note 3' },
      ],
      currentNote: { id: null, title: '', content: '' },
      editMode: false,
      searchText: '',
    };
  },
  computed: {
    filteredNotes() {
      return this.notes.filter((note) =>
        note.title.toLowerCase().includes(this.searchText.toLowerCase())
      );
    },
  },
  methods: {
    selectNote(note) {
      this.currentNote = { ...note };
      this.editMode = false;
    },
    saveNote() {
      const index = this.notes.findIndex((note) => note.id === this.currentNote.id);
      if (index !== -1) {
        this.notes[index] = { ...this.currentNote };
      }
    },
    deleteNote(note) {
      const index = this.notes.findIndex((n) => n.id === note.id);
      if (index !== -1) {
        this.notes.splice(index, 1);
        this.currentNote = { id: null, title: '', content: '' };
      }
    },
  },
  watch: {
    currentNote: {
      handler() {
        if (this.editMode) {
          this.saveNote();
        }
      },
      deep: true,
    },
  },
};
</script>

<style>
.sidebar {
  width: 200px;
  float: left;
  padding: 10px;
}

.content {
  margin-left: 220px;
  padding: 10px;
}

textarea {
  width: 100%;
  height: 300px;
}

.search{
  height: 100px;
}
</style>
