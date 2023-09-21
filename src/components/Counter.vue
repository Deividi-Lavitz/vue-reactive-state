<script setup lang="ts">
import { ref } from 'vue';

const count = ref(0);

function incrementCounter() {
  count.value++;
}

function onClick() {
  incrementCounter();
}
</script>
<template>
  <div>
    <button @click="onClick">Click Here!</button>
    <span>Was clicked {{ count }} times!</span>
  </div>
</template>
