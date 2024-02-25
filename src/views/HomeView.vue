<script setup lang="ts">
import { onMounted } from 'vue';
import SafiButton from '@/components/SafiButton.vue';
import { SpotifyApi } from '@spotify/web-api-ts-sdk';

const client_id: string = import.meta.env.VITE_SPTFY_CLIENT_ID
const client_secret: string = import.meta.env.VITE_SPTFY_CLIENT_SECRET

// credentials are optional
const sdk: SpotifyApi = SpotifyApi.withClientCredentials(client_id, client_secret);

onMounted(async () => {
  const items = await sdk.search("The Beatles", ["artist"]);
  console.log(items)
})
</script>

<template>
  <main class="flex items-center justify-center h-screen w-screen">
    <div class="grid grid-cols-2 gap-4">
      <SafiButton :title="'1'" />
      <SafiButton :title="'2'" />
      <SafiButton :title="'3'" />
      <SafiButton :title="'4'" />
    </div>
  </main>
</template>
