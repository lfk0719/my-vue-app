<template>
  <el-config-provider :locale="locale">
    <HelloWorld msg="Vite + Vue" />
  </el-config-provider>
</template>

<script setup>
import { ref } from "vue";
import HelloWorld from "./components/HelloWorld.vue";
import zhCn from "element-plus/es/locale/lang/zh-cn";
import plusZhCn from 'plus-pro-components/es/locale/lang/zh-cn'

const locale = ref({ ...zhCn, ...plusZhCn });
</script>
