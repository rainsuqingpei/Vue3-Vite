<template>
  <div>
    <!-- 路由匹配到的组件将渲染在这里 -->
    <router-link to="/">Go to Home</router-link>
    <br />
    <router-link to="/about">Go to About</router-link>
    <br />
    <router-link to="/user/111">Go to User</router-link>
    <!-- 路由匹配到的组件将渲染在这里 -->

    <div>About.vue</div>
    <div>width: {{ width }}</div>
    <div>height: {{ height }}</div>
  </div>
</template>
<script setup>
import { ref, reactive } from "vue";
import { useWindowSize } from "../components/useWindowSize";

const { width, height } = useWindowSize();
</script>
<style scoped></style>
