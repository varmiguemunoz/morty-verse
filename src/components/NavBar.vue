<script lang="ts" setup>
defineProps<{
  message: string
}>()
</script>

<template>
  <nav id="navbar-container">
    <div class="container-left-nav">
      <img src="@/assets/logo.svg" width="50" height="50" />

      <p class="message-navbar">{{ message }}</p>
    </div>

    <div class="container-rigth-nav">
      <router-link to="/login" class="link-text-navbar">Login</router-link>
    </div>
  </nav>
</template>

<style>
#navbar-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #000;
  width: 100%;
  padding: 20px;
}

.container-left-nav {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 15px;
}

.message-navbar {
  color: white;
  text-transform: capitalize;
  font-size: 18px;
  font-weight: 600;
}

.link-text-navbar {
  text-transform: capitalize;
  font-size: 18px;
  font-weight: 600;
  cursor: pointer;
}

</style>
