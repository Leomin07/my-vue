<script lang="ts">
import { defineComponent } from 'vue';
import { Button } from 'ant-design-vue';

export default defineComponent({
  name: 'TodoItem',
  props: ['todoProps'],
});
</script>

<template>
  <div class="todo-item">
    <a-checkbox>Finish</a-checkbox>
    <p>{{ todoProps?.name }}</p>
    <a-button type="primary">Delete</a-button>
  </div>
</template>

<style scoped>
.todo-item {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}
</style>
