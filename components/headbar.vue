<template>
  <div class="headerbar">
    <div class="lg:ml-[47px] md:ml-[10px] sm:ml-[2px]">
      <img src="/emojione_video-game.png" />
    </div>
    <div class="flex items-center justify-center gap-4 grid-cols-3">
      <div class="text-center text-white font-medium text-[12px]">
        <p>{{ name }}</p>
        <div
          class="bg-[#fff] rounded-lg px-[5px] flex items-center justify-center text-[#215E95] font-bold mt-[6px]"
        >
          <img src="/image 3.png" alt="" class="mr-2 w-4 h-4" />
          <p>{{ amount }}</p>
        </div>
      </div>

      <svg
        class="w-7 h-7 text-gray-800 dark:text-white"
        fill="currentColor"
        viewBox="0 0 20 20"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          fill-rule="evenodd"
          d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z"
          clip-rule="evenodd"
        ></path>
      </svg>
      <!-- <img src="/profile.png" alt="" class="img-icon" /> -->

      <svg
        class="w-6 h-6 text-gray-800 dark:text-white"
        aria-hidden="true"
        xmlns="http://www.w3.org/2000/svg"
        fill="currentColor"
        viewBox="0 0 17 14"
      >
        <path
          d="M16 2H1a1 1 0 0 1 0-2h15a1 1 0 1 1 0 2Zm0 6H1a1 1 0 0 1 0-2h15a1 1 0 1 1 0 2Zm0 6H1a1 1 0 0 1 0-2h15a1 1 0 0 1 0 2Z"
        ></path>
      </svg>
    </div>
  </div>
</template>

<style>
.headerbar {
  @apply bg-blue-800 flex justify-between lg:px-[49px] md:px-[20px] sm:px-[10px]  px-3;
}
.img-icon {
  @apply w-12 h-12;
}
</style>

<script setup lang="ts">
defineProps<{
  amount?: string;
  name?: string;
}>();
</script>
