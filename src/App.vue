<template>
<header>
    <div class="menu-esquerdo">
      <span>Home</span>
      <span>|</span>
      <span>Jogadores</span>
      <span>|</span>
      <span>Times</span>
    </div>
    <div class="menu-direito">
      <span>Sair</span>
    </div>
  </header>
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

header,
footer {
  height: 10%;
  background-color: #db7093;
  color: black;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-left: 20px;
}
header span {
  padding-left: 20px;
  padding-right: 20px;
}
main {
  height: 80%;
  background-color: crimson;
}
</style>
