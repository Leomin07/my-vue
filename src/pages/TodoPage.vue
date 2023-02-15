<script lang="ts">
import { defineComponent, ref } from 'vue';
import Footer from '../components/Main/Footer.vue';
import Header from '../components/Main/Header.vue';
import TodoItem from '../components/Todo/TodoItem.vue';
import { ITodo } from '../types/interface';

export default defineComponent({
  name: 'TodoPage',
  components: { Header, Footer, TodoItem },
  setup() {
    const data = ref<ITodo[]>([
      {
        id: 1,
        name: 'minh',
        isFinished: false,
      },
      {
        id: 2,
        name: 'minh',
        isFinished: false,
      },
      {
        id: 3,
        name: 'minh',
        isFinished: false,
      },
      {
        id: 4,
        name: 'minh',
        isFinished: false,
      },
    ]);

    return {
      data,
    };
  },
});
</script>

<template>
  <Header />
  <TodoItem
    v-for="todo in data"
    :key="todo.id"
    v-bind:todoProps="todo"
  ></TodoItem>
  <Footer />
</template>

<style></style>
