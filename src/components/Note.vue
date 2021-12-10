<template>
  <h1>Note Content {{ content }}</h1>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component';

@Options()
export default class Note extends Vue {
  public get content() {
    return 'Lorem Ipsum this is content';
  }
}
</script>
