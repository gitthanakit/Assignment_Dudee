<template>
  <div class="hover-icon" v-for="(item, index) in iconsmall">
    <!-- <img :src="item.url" alt="" class="image-icon" /> -->
    <Icon :name="item.iconname" class="iconsize"></Icon>
    <p>{{ item.name }}</p>
  </div>
</template>

<script setup lang="ts">
const iconsmall = ref([
  {
    url: "/simple-icons_gamemaker.svg",
    iconname: "simple-icons:gamemaker",
    name: "ทัวร์นาเมนต์ทั้งหมด",
  },
  {
    url: "/mdi_announcement.svg",
    iconname: "mdi:megaphone",
    name: "ประกาศ",
  },
  {
    url: "/material-symbols_rewarded-ads-rounded.svg",
    iconname: "mage:trophy-star-fill",
    name: "ผลรางวัล",
  },
  {
    url: "/icon-park-solid_ranking-list.svg",
    iconname: "icon-park-solid:alignment-bottom-center",
    name: "ตารางอันดับ",
  },
]);
</script>

<style>
.hover-icon {
  @apply lg:py-3 sm:py-1 lg:mx-4 sm:mx-2 mx-1 sm:px-10 px-3 my-2 rounded-lg text-center hover:bg-[#1F2B6A] hover:text-[#FDD835] lg:text-base md:text-sm sm:text-sm text-[12px];
}
.image-icon {
  @apply block mx-auto md:w-12 sm:w-10 w-8;
}
.iconsize {
  @apply lg:text-[46px] md:text-[40px] sm:text-[36px] text-[30px];
}
</style>
