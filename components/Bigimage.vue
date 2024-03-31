<template>
  <div class="py-0">
    <img :src="url" alt="" class="w-full lg:h-96 md:h-60 sm:h-auto" />
  </div>
</template>

<script setup lang="ts">
defineProps<{
  url?: string;
}>();
</script>
