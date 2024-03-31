<template>
  <div class="tab-noti">
    <div class="flex items-center justify-center ml-12">
      <span class="span-icon">
        <p>{{ no }}</p>
      </span>
      <img :src="img" class="profile-icon" />
      <p class="text-white">{{ name }}</p>
    </div>
    <div>
      <button type="button" class="bttn-noti">{{ imgbttn }}</button>
    </div>
  </div>
</template>

<style>
.tab-noti {
  @apply px-3 bg-gradient-to-r from-[#5394FF] to-[#146CFB] w-full shadow-md rounded-xl flex justify-between py-[10.5px] px-[16px];
}
.bttn-noti {
  @apply w-48 h-20 rounded-lg font-bold text-xl text-[#C5A000] bg-[radial-gradient(ellipse_at_center,_var(--tw-gradient-stops))] from-[#FDD835] to-[#D0B022] hover:bg-yellow-500;
}
.profile-icon {
  @apply rounded-md mr-1 ml-3 h-14 w-14;
}
.span-icon {
  @apply bg-stone-800 py-2 px-4 rounded-full bg-[#DFDFDF] text-[#666666] font-medium;
}
</style>

<script setup lang="ts">
defineProps<{
  no?: string;
  img?: string;
  name?: string;
  imgbttn?: string;
}>();
</script>
