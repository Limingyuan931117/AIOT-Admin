<script setup lang="ts">
import { ref } from "vue";
defineOptions({
  name: "Welcome"
});
const value = ref(0);
</script>

<template>
  <div>
    <h1>首页</h1>
    <div>
      <el-input v-model="value" />
    </div>
  </div>
</template>
