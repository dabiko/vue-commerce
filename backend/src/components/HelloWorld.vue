<script setup>
import { ref, computed } from 'vue'
import store from "../store/index.js";

defineProps({
  msg: String,
})

const test = computed(() => store.state.test);

const count = ref(0)
</script>

<template>
  <div class="card">
      {{ test }}
  </div>
</template>


