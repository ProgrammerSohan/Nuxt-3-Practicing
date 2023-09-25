<template>
  
 <!--  <HomeWelcome /> -->

<button @click="toggle">Toggle</button>
<component :is="MyComponent" />


</template>
<script setup>
const MyComponent = ref(resolveComponent("Counter"));

function toggle(){
MyComponent.value = resolveComponent("HomeWelcome");


}

</script>

 