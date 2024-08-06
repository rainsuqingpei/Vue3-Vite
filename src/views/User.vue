<template>
  <div>
    <!-- 路由匹配到的组件将渲染在这里 -->
    <router-link to="/">Go to Home</router-link>
    <br />
    <router-link to="/about">Go to About</router-link>
    <br />
    <router-link to="/user/111">Go to User</router-link>
    <!-- 路由匹配到的组件将渲染在这里 -->

    <div>User.vue</div>
  </div>
</template>

<script setup>
import { useRoute } from "vue-router";
console.log(useRoute().params.itemId);
</script>
<style scoped></style>
