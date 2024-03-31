<template>
  <div class="hover-icon">
    <!-- <Icon :name="url" size="50px" class="text-center" /> -->
    <img :src="url" alt="" class="block mx-auto" />
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
  @apply py-3 px-8 my-2 rounded-lg text-center hover:bg-[#1F2B6A] hover:text-[#FDD835];
}
</style>
