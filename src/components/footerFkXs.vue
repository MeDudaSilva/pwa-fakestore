<script setup>
import Account from "vue-material-design-icons/Account.vue";
import Star from "vue-material-design-icons/Star.vue";
import Home from "vue-material-design-icons/Home.vue";
</script>

<template>
  <footer>
    <div class="conheca-nos">
      <Star size="50px" />
    </div>
    <div class="home">
      <Home size="50px"/>
    </div>
    <div class="sociais">
      <Account size="50px"/>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  justify-content: space-around;
  background-color: rgb(231, 162, 11);
  width: 100%;
  height: 15vh;
  align-items: center;
  position: fixed;
  bottom: 0%;
}
img {
  width: 10vh;
}
</style>
