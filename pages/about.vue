<template>
    <div>
      <ul>
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li>About</li>
        <li><NuxtLink to="/contacts">Contacts</NuxtLink></li>
        <li><NuxtLink to="/items">Items</NuxtLink></li>
      </ul>
      <div>pos: {{ x }}, {{ y }}</div>
      <button style="border: 1px solid #333; padding: 5px;" @click="sendMessage">Send message to Contacts</button>
      
    </div>
</template>

<script setup>
  
  definePageMeta({
    layout: "default",
  })

  const { x, y } = useMouse()
    
  onMounted(() => {
    console.log(`About onMounted`);
  })

  const sendMessage = () => {
    console.log(`About sendMessage...`);
  }

</script>

<style scoped>

</style>