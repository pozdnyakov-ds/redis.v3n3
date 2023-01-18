<template>
    <div>
      <ul>
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li>Contacts</li>
        <li><NuxtLink to="/items">Items</NuxtLink></li>
      </ul>
      <button style="border: 1px solid #333; padding: 5px;" @click="sendMessage">Send message to About</button>
    </div>
</template>

<script setup>
  
  definePageMeta({
    layout: "default",
  })
 
  onMounted(() => {
    console.log(`Contacts onMounted`);
  })

  const sendMessage = () => {
    console.log(`Contacts sendMessage...`);
  }

</script>

<style scoped>

</style>