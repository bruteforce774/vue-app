<script setup>
import { ref, reactive } from 'vue'

const message = ref('Hi!')

const counter = reactive({
  count: 0
})
</script>

<template>
  <h1>{{ message }}</h1>
  <button @click="counter.count++">Count is: {{ counter.count }}</button>
  &nbsp;<button @click="counter.count = 0">Reset</button>
</template>

<style scoped></style>
