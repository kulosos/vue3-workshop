<template>
  <h2>HelloWorld</h2>
  <div>{{ label }} {{ count }}</div>
  <button @click="increment">+1</button>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component';

@Options({
  watch: {
    count: (value) => {
      console.log(value);
    },
  },
})
export default class HelloWorld extends Vue {
  public count = 0;

  public increment() {
    this.count++;
  }

  public get label(): string {
    return 'Label: ';
  }

  public counter(value: number) {
    console.warn('counter: ', this.count);
  }
}
</script>

<style scoped></style>
