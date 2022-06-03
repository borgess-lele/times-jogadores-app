<template>
  <header>
    <div class="menu-esquerdo">
      <span> <RouterLink to="/">Home</RouterLink></span>
      <span>|</span>
      <span><RouterLink to="/times">Times </RouterLink></span>
      <span>|</span>
      <span><RouterLink to="/jogadores">Jogadores </RouterLink></span>
    </div>
    <div class="menu-direito">
      <span>Sair</span>
    </div>
  </header>
</template>

<style>
header {
  height: 10%;
  background-color: #1b6e06;
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
</style>
