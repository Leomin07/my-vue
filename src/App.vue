<script lang="ts">
import { defineComponent } from 'vue';
import TodoPage from './pages/TodoPage.vue';

export default defineComponent({
  name: 'App',
  components: {
    TodoPage,
  },
  setup() {},
});
</script>

<template>
  <div>
    <TodoPage />
  </div>
</template>

<style scoped></style>
