<script setup>
import Account from "vue-material-design-icons/Home.vue";
</script>

<template>
  <footer>
    <div class="conheca-nos">
      <Account/>
    </div>
    <div class="sociais">
      <div class="credito"><img src="@/assets/logoFakeStore.png" alt="" /></div>
    </div>
    <div class="pagamento">
      <div class="credito"><img src="@/assets/logoFakeStore.png" alt="" /></div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  justify-content: space-around;
  background-color: rgb(255, 255, 255);
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
