<template>
  <div class="py-0">
    <img :src="url" alt="" class="w-full h-80" />
  </div>
</template>

<script setup lang="ts">
defineProps<{
  url?: string;
}>();
</script>
