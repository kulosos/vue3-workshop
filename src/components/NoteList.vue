<template>
  <h1>NoteList Component {{ label }}</h1>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component';

@Options()
export default class NoteList extends Vue {
  public get label() {
    return 'MyLabel';
  }
}
</script>
