<script setup>
import HeaderComp from "@/components/template/HeaderComp.vue";
</script>

<template>
  <HeaderComp />
  <RouterView />
</template>

<style>
@import "@/assets/base.css";

#app {
  max-width: 1280px;
  margin: 0 auto;
  height: 100vh;
  /* padding: 2rem; */

  font-weight: normal;
}
a {
  color: inherit;
  text-decoration: none;
}

footer {
  height: 10%;
  background-color: #1b6e06;
  color: black;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 20px;
}

main {
  height: 80%;
  background-color: rgb(97, 236, 4);
}
</style>
