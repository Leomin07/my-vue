<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Header',
});
</script>

<template lang="">
  <div>
    <span>Project Learn Vue3</span>
  </div>
</template>
<style scoped>
div {
  text-align: center;
  background-color: #777;
  padding: 10px 0;
  position: absolute;
  bottom: 0;
  width: 100%;
}

span {
  color: #fff;
}
</style>
