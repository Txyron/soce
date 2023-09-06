<script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <router-link to="/about">À propos</router-link>
    <router-link to="/welcome">Welcome</router-link>
    
    <the-welcome/>
    <router-view></router-view>
  </main>
</template>
