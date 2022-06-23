<template>
  <div class="container">
    <GlobalHeaderVue :user="currentUser" />
    <ColumnListVue :list="testData" />
  </div>
</template>

<script setup lang="ts">
import "bootstrap/dist/css/bootstrap.min.css";
import ColumnListVue, { ColumnProps } from "@/components/ColumnList.vue";
import GlobalHeaderVue, { UserProps } from "@/components/GlobalHeader.vue";
import logo from "@/assets/logo.png";
const testData: ColumnProps[] = [
  {
    id: 1,
    title: "test1专栏",
    description: "啊实打实大苏打实打实打算",
    avatar: logo,
  },
  {
    id: 2,
    title: "test2专栏",
    description: "啊实打实大苏打实打实打算",
    avatar: logo,
  },
  {
    id: 3,
    title: "test3专栏",
    description: "啊实打实大苏打实打实打算",
    avatar: logo,
  },
  {
    id: 4,
    title: "test4专栏",
    description: "啊实打实大苏打实打实打算",
    avatar: logo,
  },
];
const currentUser: UserProps = {
  isLogin: true,
  name: "cxl",
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
