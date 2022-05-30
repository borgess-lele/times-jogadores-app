<template>
  <header>
    <span class="texto-header">Home</span>
    <span class="separador">|</span>
    <span class="texto-header">Jogadores</span>
    <span class="separador">|</span>
    <span class="texto-header">Times</span>
    <span class="separador">|</span>
    
    </header>
  <main>Main</main>
  <footer>Rodapé</footer>
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
}

main {
  height: 80%;
  background-color: crimson;
}
</style>
