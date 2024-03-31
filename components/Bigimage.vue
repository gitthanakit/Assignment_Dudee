<template>
  <div class="py-0">
    <img :src="url" alt="" class="w-full 2xl:h-2/5 lg:h-96 md:h-60 sm:h-auto" />
  </div>
</template>

<script setup lang="ts">
defineProps<{
  url?: string;
}>();
</script>
