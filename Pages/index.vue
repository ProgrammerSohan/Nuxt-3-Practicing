<template>
   <div>
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="about">About</NuxtLink>
    
    <button @click="moveToAbout">Take me to about page</button>
    Hello Sohan! Index Page.
   </div>
</template>
<script setup>
    function moveToAbout(){

        navigateTo("about");
    }

</script>
