<template>
  
 <!--  <HomeWelcome /> -->

<button @click="toggle">Toggle</button>
<component :is="MyComponent" />


</template>
<script setup>
const MyComponent = shallowRef(resolveComponent("Counter"));

function toggle(){
  console.log(MyComponent.value.name);
MyComponent.value = resolveComponent("HomeWelcome");


}

</script>

 