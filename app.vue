<template>
  

  <HomeWelcome />
<component :is="Counter" />


</template>
<script setup>
const Counter = resolveComponent("Counter");

</script>

 