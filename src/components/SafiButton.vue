<script setup lang="ts">
defineProps<{
  title: string
}>()
</script>

<template>
  <div class="flex flex-row 
              justify-center items-center w-[200px] h-[200px] 
              border-2 border-slate-600/30 rounded-2xl
              hover:bg-slate-600/10
              ">
    <h1 class="text-green-500 text-2xl">{{ title }}</h1>
  </div>
</template>

<style scoped></style>
