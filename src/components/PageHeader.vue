<template>
  <header id="header">
    <div class="elements">
      <img class="logo-image" src="@/assets/logo.png" alt="" />
      <span class="logo-title">DRAKUNATH</span>
    </div>
    <nav class="nav">
      <span class="nav-item">Início</span>
      <span class="nav-item">Sobre</span>
      <span class="nav-item">Social Media</span>
      <span class="nav-item">Outros</span>
    </nav>
  </header>
</template>

<script setup lang="ts"></script>

<style scoped>
#header {
  background-color: rgba(0, 0, 0, 0.9);
  border-radius: 12px;
  height: 55px;

  display: flex;
  padding-inline: 1rem;
}

.elements {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.elements img {
  height: 40px;
}

.elements span {
  color: #bd0171;
  font-weight: 400;
  font-size: 1.4rem;
}

.nav {
  display: flex;
  justify-content: center;
  flex: 1;
}

.nav-item {
  cursor: pointer;
  color: #bd0171;
  font-weight: 600;
  font-size: 1.3rem;
  border-bottom: 2px solid transparent;
  padding-block: 0.65rem;
  padding-inline: 1.2rem;
}

.nav-item:hover {
  filter: brightness(1.5);
  border-color: #bd0171;
}
</style>
