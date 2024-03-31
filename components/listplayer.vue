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
        :class="[
          index == 0
            ? 'grid-temp-cols cols-top3 list-block bg-[#FDD835] border-[#F39E09]'
            : index == 1
            ? 'grid-temp-cols cols-top3 list-block bg-[#CDCDE9] border-[#CDCDE9]'
            : index == 2
            ? 'grid-temp-cols cols-top3 list-block bg-[#FA6B25] border-[#F9914A]'
            : 'grid-temp-cols list-block',
        ]"
        v-for="(item, index) in listplayer"
      >
        <img class="img-no" :src="item.image" alt="" />
        <div class="flex">
          <img class="img-profile-list" src="/profile-image.png" alt="" />
          <div class="text-point-list">{{ item.name }}</div>
        </div>
        <p class="text-point-list text-[#C96203]">{{ item.point }}</p>
        <div class="text-point-list">
          <p
            :class="[
              index == 0
                ? 'bg-[#FDD835] reward-list-top3'
                : index == 1
                ? 'bg-[#CDCDE9] reward-list-top3'
                : index == 2
                ? 'bg-[#D34C46] reward-list-top3'
                : '',
            ]"
          >
            {{ item.rewards }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const listplayer = ref([
  {
    image: "/no1.png",
    name: "TIGER88RI0399",
    point: "3500",
    rewards: "IPHONE12",
  },
  {
    image: "/no2.png",
    name: "RGRP8GG01577",
    point: "3200",
    rewards: "VR",
  },
  {
    image: "/no3.png",
    name: "KGTR3311190122",
    point: "3000",
    rewards: "Mouse Gaming",
  },
  {
    image: "/no4.png",
    name: "JKL0023441848",
    point: "2000",
    rewards: "200 coins",
  },
  {
    image: "/no5.png",
    name: "RWS2II77102641",
    point: "1500",
    rewards: "100 coins",
  },
  {
    image: "/no6.png",
    name: "AZQ82II4102672",
    point: "1450",
    rewards: "50 coins",
  },
]);
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
  @apply sm:w-36 w-[96px] px-1 py-1 rounded-full text-white break-all text-center;
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
