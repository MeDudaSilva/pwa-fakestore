<script setup>
  import { useMonitor } from '@/composables/monitor';

  const { menu } = useMonitor();  
  const { footerFk} = useMonitor();

</script>

<template>
  <div>
    <component :is="menu" />
    <main>
      <router-view />
    </main>
    <footer>
    <component :is="footerFk" />
      <p>Copyright &copy; 2024</p>
    </footer>
  </div>
</template>
