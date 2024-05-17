<script setup lang="ts">
defineProps<{
  message: string
}>()
</script>

<template>
  <div class="container-header">
    <div class="container-left">
      <div class="container-text-left">
        <h1 class="header-text">{{ message }}</h1>
        <p class="header-subtext">Discover all the characters you've never seen before 🚀</p>
      </div>

      <button >login</button>
    </div>

    <div class="container-right">
      <img src="@/assets/rick-4k.png" width="500px" height="500px" class="img-header" />
    </div>
  </div>
</template>

<style>
.container-header {
  max-width: 1114px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
}

.container-left {
  width: 50%;
  display: flex;
  flex-direction: column;
  gap: 70px;
}

.container-right {
  width: 50%;
}

.container-text-left {
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: start;
  gap: 30px;
}

.header-text {
  font-size: 72px;
  font-weight: 600;
  line-height: 72px;
  color: black;
}

.header-subtext {
  font-size: 18px;
  font-weight: 500;
  line-height: 20px;
}

.img-header {
  border-radius: 300px;
  object-fit: cover;
}
</style>
