<template>
  <NoteList />
  <Note />
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component';
import Note from './components/Note.vue';
import NoteList from './components/NoteList.vue';

@Options({
  components: {
    Note
    NoteList,
  },
})
export default class App extends Vue {}
</script>
