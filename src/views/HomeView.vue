<script lang="ts" setup>
import NavBar from '@/components/NavBar.vue'
import MainHeader from '@/components/MainHeader.vue'
</script>

<template>
  <main>
    <NavBar message="Rick & morty website" />

    <div class="header-principal-container">
      <MainHeader message="Enter into the world of rick and morty" />
    </div>
  </main>
</template>

<style>
.header-principal-container {
  width: 100%;
  height: 91vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 50px;
}
</style>
