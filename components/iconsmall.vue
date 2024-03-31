<template>
  <div class="hover-icon">
    <!-- <Icon :name="url" size="50px" class="text-center" /> -->
    <img :src="url" alt="" class="image-icon" />
    <p>{{ iconname }}</p>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  url?: string;
  iconname?: string;
}>();
</script>

<style>
.hover-icon {
  @apply lg:py-3 sm:py-1 lg:px-20 md:px-16 sm:px-10 px-3 my-2 rounded-lg text-center hover:bg-[#1F2B6A] hover:text-[#FDD835] lg:text-base md:text-sm sm:text-sm text-[12px];
}
.image-icon {
  @apply block mx-auto md:w-12 sm:w-10 w-8;
}
</style>
