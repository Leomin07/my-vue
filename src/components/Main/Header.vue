<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Header',
});
</script>

<template>
  <div class="header">
    <nav>
      <ul>
        <li>Home</li>
        <li>Todo</li>
        <li>About</li>
      </ul>
    </nav>
  </div>
</template>

<style scoped>
.header {
  text-align: center;
  padding: 20px 0;
  background-color: #777;
}
nav {
}
ul {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

li {
  color: #fff;
  list-style-type: none;
  cursor: pointer;
}

li:hover {
  color: #c3ddef;
  transition: all 0.3s;
}
</style>
