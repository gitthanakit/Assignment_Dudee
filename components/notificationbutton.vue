<template>
  <div class="tab-noti">
    <div class="div-cover-noti">
      <span class="span-icon">
        <p>{{ no }}</p>
      </span>
      <img :src="img" class="profile-icon" />
      <p class="player-name">{{ name }}</p>
    </div>
    <div>
      <button type="button" class="bttn-noti">{{ imgbttn }}</button>
    </div>
  </div>
</template>

<style>
.tab-noti {
  @apply px-3 bg-gradient-to-r from-[#5394FF] to-[#146CFB] w-full shadow-md md:rounded-xl flex justify-between py-[10.5px] sm:px-[16px] px-2;
}
.div-cover-noti {
  @apply flex items-center justify-center lg:ml-12 md:ml-6;
}
.bttn-noti {
  @apply lg:w-48 md:w-36 sm:w-36 w-28 lg:h-20 md:h-16 h-14 rounded-lg font-bold lg:text-xl md:text-lg text-base text-[#C5A000] bg-[radial-gradient(ellipse_at_center,_var(--tw-gradient-stops))] from-[#FDD835] to-[#D0B022] hover:bg-yellow-500;
}
.profile-icon {
  @apply mr-1 sm:ml-3 ml-2 sm:h-14 sm:w-14 w-11 h-11;
}
.span-icon {
  @apply bg-stone-800 sm:py-2 sm:px-4 py-1 px-3 rounded-full bg-[#DFDFDF] text-[#666666] font-medium;
}
.player-name {
  @apply text-white break-all lg:text-lg md:text-base text-sm;
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
