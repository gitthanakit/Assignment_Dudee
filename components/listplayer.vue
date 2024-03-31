<template>
  <div class="div-cover-list">
    <div class="grid-temp-cols topic-text-list">
      <p>อันดับ</p>
      <p>ชื่อผู้เล่น</p>
      <p class="specific-width-column">คะแนน</p>
      <p class="specific-width-column">รางวัล</p>
    </div>
    <div>
      <div
        class="grid-temp-cols cols-top3 list-block bg-[#FDD835] border-[#F39E09]"
      >
        <img class="img-no" src="/no1.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">TIGER88RI0399</div>
        </div>
        <p class="text-point-list text-[#C96203]">3500</p>
        <div class="text-point-list">
          <p class="bg-[#FDD835] reward-list-top3">IPHONE12</p>
        </div>
      </div>
      <div
        class="grid-temp-cols cols-top3 list-block bg-[#CDCDE9] border-[#CDCDE9]"
      >
        <img class="img-no" src="/no2.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">RGRP8GG01577</div>
        </div>
        <p class="text-point-list text-[#C96203]">3200</p>
        <div class="text-point-list">
          <p class="bg-[#CDCDE9] reward-list-top3">VR</p>
        </div>
      </div>
      <div
        class="grid-temp-cols cols-top3 list-block bg-[#FA6B25] border-[#F9914A]"
      >
        <img class="img-no" src="/no3.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">RGRP8GG01577</div>
        </div>
        <p class="text-point-list text-[#C96203]">3000</p>
        <div class="text-point-list">
          <p class="bg-[#D34C46] reward-list-top3">Mouse Gaming</p>
        </div>
      </div>
      <div class="grid-temp-cols list-block">
        <img class="img-no" src="/no4.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">RGRP8GG01577</div>
        </div>
        <p class="text-point-list text-[#C96203]">2000</p>
        <div class="text-point-list">
          <p>200 coins</p>
        </div>
      </div>
      <div class="grid-temp-cols list-block">
        <img class="img-no" src="/no5.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">RGRP8GG01577</div>
        </div>
        <p class="text-point-list text-[#C96203]">1500</p>
        <div class="text-point-list">
          <p>100 coins</p>
        </div>
      </div>
      <div class="grid-temp-cols list-block">
        <img class="img-no" src="/no4.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">RGRP8GG01577</div>
        </div>
        <p class="text-point-list text-[#C96203]">1450</p>
        <div class="text-point-list">
          <p>50 coins</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  no?: string;
  img?: string;
  name?: string;
  imgbttn?: string;
}>();
</script>

<style>
.topic-text-list p {
  @apply font-normal md:text-base sm:text-sm text-[11px];
}
.specific-width-column {
  @apply sm:w-36 text-center;
}
.div-cover-list {
  @apply py-3 sm:px-[3px] px-0 bg-[#F4F4F4]  rounded-md text-[#A3AEBE];
}
.cols-top3 {
  @apply border-4 bg-opacity-25;
}

.reward-list-top3 {
  @apply sm:w-36 w-[96px] px-2 py-1 rounded-full text-white break-all text-center;
}
.grid-temp-cols {
  @apply grid sm:gap-2 text-xs md:px-3 px-2;
  grid-template-columns: 0.2fr 3fr 1fr 1fr;
  grid-auto-flow: column;
}
@media only screen and (max-width: 639px) {
  .grid-temp-cols {
    grid-template-columns: 0.2fr 1fr 0.4fr 0.8fr;
    grid-auto-flow: column;
  }
}
.text-point-list {
  @apply flex items-center justify-center font-semibold break-all md:text-base sm:text-sm text-[11px] sm:w-36;
}
.list-block {
  @apply px-4 py-5 rounded-lg mx-1 my-1 text-black;
}
.img-no {
  @apply md:w-8 md:h-8 w-7 h-7 rounded-full;
}
.img-profile-list {
  @apply md:w-10 md:h-10 w-8 h-8 rounded-full;
}
</style>
