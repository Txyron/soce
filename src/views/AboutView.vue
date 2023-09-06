<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import AboutView from '../components/About.vue'

</script>

<template>
  <main>
    <router-link to="about">Avis</router-link>
    <router-link to="/welcome">Welcome</router-link>
<TheWelcome/>
<AboutView/>
  </main>
</template>
