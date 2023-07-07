<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button
      type="button"
      class="hover:border-white border-2 border-transparent p-3 rounded-xl"
      @click="count++"
    >
      count is {{ count }}
    </button>
  </div>
</template>
