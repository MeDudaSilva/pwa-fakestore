<script setup>
import Account from "vue-material-design-icons/Account.vue";
</script>

<template>
  <footer>
    <div class="conheca-nos">
      <div class="credito"><img src="@/assets/logoFakeStore.png" alt="" /></div>
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
  background-color: rgb(255, 238, 3);
  width: 100%;
  height: 200px;
  align-items: center;
  bottom: 0%;
  position: fixed;
}
img {
  width: 10vh;
}
</style>
