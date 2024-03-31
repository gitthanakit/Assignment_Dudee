<template>
  <div
    class="mx-[8px] my-[20px] py-3 px-5 bg-[#F4F4F4] px-[3px] rounded-md text-[#A3AEBE]"
  >
    <div class="grid-temp-cols">
      <p>อันดับ</p>
      <p>ชื่อผู้เล่น</p>
      <p>คะแนน</p>
      <p>รางวัล</p>
    </div>
    <div>
      <div
        class="grid-temp-cols list-block bg-[#FDD835] border-4 border-[#F39E09] bg-opacity-25"
      >
        <img class="img-no" src="/no1.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">TIGER88RI0399</div>
        </div>
        <p class="text-point-list text-[#C96203]">3500</p>
        <div class="text-point-list">
          <p class="bg-[#FDD835] px-6 py-1 rounded-full text-white">IPHONE12</p>
        </div>
      </div>
      <div
        class="grid-temp-cols list-block bg-[#CDCDE9] border-4 border-[#CDCDE9] bg-opacity-25"
      >
        <img class="img-no" src="/no2.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">RGRP8GG01577</div>
        </div>
        <p class="text-point-list text-[#C96203]">3200</p>
        <div class="text-point-list">
          <p class="bg-[#CDCDE9] px-10 py-1 rounded-full text-white">VR</p>
        </div>
      </div>
      <div
        class="grid-temp-cols list-block bg-[#FA6B25] border-4 border-[#F9914A] bg-opacity-25"
      >
        <img class="img-no" src="/no3.png" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">RGRP8GG01577</div>
        </div>
        <p class="text-point-list text-[#C96203]">3000</p>
        <div class="text-point-list">
          <p class="bg-[#D34C46] px-3 py-1 rounded-full text-white">
            Mouse Gaming
          </p>
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
.grid-temp-cols {
  @apply grid gap-2 text-xs;
  grid-template-columns: 0.2fr 3fr 0.5fr 0.5fr;
  grid-auto-flow: column;
}
.text-point-list {
  @apply flex items-center justify-center text-xs font-semibold;
}
.list-block {
  @apply px-4 py-5 rounded-lg mx-1 my-1 text-black;
}
.img-no {
  @apply w-8 h-8 rounded-full flex items-center justify-center;
}
.img-profile-list {
  @apply w-10 h-10 rounded-full mr-2;
}
</style>
