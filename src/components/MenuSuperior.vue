<script setup>
import { ref } from 'vue';

import CartPlus from 'vue-material-design-icons/CartPlus.vue';
import Account from 'vue-material-design-icons/Account.vue';
import Menu from 'vue-material-design-icons/Menu.vue';

const menuAberto = ref(false);
</script>

<template>
    <header>
      <div class="header--logo">
        <img src="@/assets/logoFakeStore.png" alt="Logo" />
        <h1>FakeStore</h1>
      </div>
      <nav>
        <ul :class="menuAberto ? 'menu' : ''">
          <li>Home</li>
          <li>Eletrônicos</li>
          <li>Jóias</li>
          <li>Masculino</li>
          <li>Feminino</li>
        </ul>
      </nav>
      <div class="header--icons">
        <Account />
        <CartPlus />
        <Menu class="menu-hamburger" @click="menuAberto = !menuAberto" />
      </div>
    </header>
  </template>

<style scoped>
h1{
    color: rgb(255, 0, 212);
}
header {
  background: #000000;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
  padding: 0.2rem 1rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom:2px solid rgb(255, 238, 3);
  color: rgb(255, 238, 3);
}

.header--logo {
  display: flex;
  align-items: center;
}
.header--logo img {
  width: 5rem;
  height: 2.5rem;
  margin-right: 0.5rem;
}
nav ul {
  display: flex;
  gap: 1rem;
}
nav li {
  list-style: none;
}

.header--icons {
  display: flex;
  gap: 1rem;
}
.menu-hamburger {
  display: none;
}

@media (max-width: 768px) {
  nav ul {
    display: none;
  }
  .menu-hamburger {
    display: block;
  }

  nav .menu {
    display: flex;
    flex-direction: column;
    position: absolute;
    background-color: rgb(255, 0, 212);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
    border-radius: 10px;
    right: 0;
    text-align: right;
    padding: 10px 16px;
  }
  nav .menu li {
    display: block;
    margin-top: 12px;
  }
}
</style>