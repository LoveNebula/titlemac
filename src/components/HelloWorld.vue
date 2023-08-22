<script setup lang="ts">
import { IS } from './inter';
import { ref } from 'vue'

defineProps<{ msg: string , dieds: string}>()
defineEmits<{ msg: string ,}>()
const count = ref(0)
const am: IS = {
  name: 'axy',
  age: 1,
  sex: "男"
}
console.log(am);

</script>

<template>
  <h1>{{ msg }}</h1>
  <h1>{{ am.sex }}</h1>
  {{ count }}
  {{ dieds }}
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
