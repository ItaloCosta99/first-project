<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import HomeHeader from '../components/HomeHeader.vue'
</script>

<template>
  <main>
    <HomeHeader v-show="showHeader" />
    <div>Nome: {{ nome }}</div>
    <TheWelcome />
  </main>
</template>

<script>
export default {
  data() {
    return {
      showHeader: false,
      nome: 'Teste'
    }
  }
}
</script>
