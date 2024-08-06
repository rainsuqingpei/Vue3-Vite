<template>
  <div>
    <!-- 路由匹配到的组件将渲染在这里 -->
    <router-link to="/">Go to Home</router-link>
    <br />
    <router-link to="/about">Go to About</router-link>
    <br />
    <router-link to="/user/111">Go to User</router-link>
    <!-- 路由匹配到的组件将渲染在这里 -->

    <div>Home.vue</div>
    <p>aaa:{{ aaa }}</p>
    <p>bbb:{{ bbb }}</p>
    <button @click="addA">aaa加一</button>
    <button @click="addB">bbb加一</button>
  </div>
</template>
<script setup>
import { ref, reactive } from "vue";
let aaa = ref(5);
const bbb = ref(10);
function addA() {
  aaa.value++;
  console.log(aaa.value);
  console.log(window.sqp);
}
function addB() {
  bbb.value++;
}
</script>
<style scoped></style>
