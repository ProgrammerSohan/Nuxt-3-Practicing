<template>
  
 <!--  <HomeWelcome /> -->

<button @click="toggle">Toggle</button>

<div v-if="MyComponent === 'welcome'" >
  <HomeWelcome />

 </div>
<Counter v-else />


<!-- <component :is="MyComponent" /> -->

</template>
<script setup>
//const MyComponent = shallowRef(resolveComponent("Counter"));
const MyComponent = ref("counter");


function toggle(){
 
//MyComponent.value = resolveComponent("HomeWelcome");
MyComponent.value = "welcome";


}

</script>

 