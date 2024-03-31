<template>
  <div class="px-[22px]">
    <div class="flex justify-between pt-[16px] pb-[22px]">
      <button class="bttn-visit-event">
        <svg
          class="arrow-bttn-event"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 11 10"
        >
          <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M10 5H1m0 0 4 4M1 5l4-4"
          ></path>
        </svg>
        <p>ทัวร์นาเมนต์ บี</p>
      </button>
      <div class="time-date-event">หมดเวลากิจกรรม</div>
    </div>
    <div class="div-cover-cardlist">
      <div class="div-grid-cover-card grid-cols-3">
        <div
          :class="[
            index == 0
              ? 'large-card-frame large-card-frame-yellow'
              : index == 1
              ? 'large-card-frame large-card-frame-grey'
              : 'large-card-frame large-card-frame-orange',
          ]"
          v-for="(item, index) in cardlist.slice(0, 3)"
        >
          <p class="no-reward large-no">{{ index + 1 }}<sup>th</sup></p>
          <img :src="item.image" alt="" class="large-card-img" />
          <p class="large-card-text-score">Score</p>
          <p class="large-card-score">{{ item.point }}</p>
          <p class="large-card-awards">{{ item.rewards }}</p>
          <p class="large-card-awards">{{ item.ticketamount }}</p>
        </div>
      </div>

      <div class="div-grid-cover-card grid-cols-4 my-6">
        <div
          class="small-card-frame"
          v-for="(item, index) in cardlist.slice(3)"
        >
          <p class="no-reward">{{ index + 4 }}<sup>th</sup></p>
          <img :src="item.image" alt="" class="small-card-img" />
          <p>{{ item.rewards }}</p>
        </div>
      </div>
    </div>
    <div>
      <article class="text-pretty text-detail-spacebuttom">
        <p>ทัวร์นาเมนต์แข่งขันยอดเล่นเกมออนไลน์</p>
        <p>
          เริ่มกิจกรรมวันที่ 19 มกราคม 2567 สิ้นสุดกิจกรรมและแจกรางวัล วันที่ 29
          มกราคม 2567
        </p>
      </article>
      <article class="text-pretty text-detail-spacebuttom">
        <p>กติกาการแข่งขัน</p>
        <ol class="list-decimal list-outside">
          <li>แข่งขันยอดเล่นเกมออนไลน์</li>
          <li>แจกรางวัลให้ผู้เล่นที่ได้ลำดับที่ 1, 2, 7</li>
        </ol>
      </article>
      <article class="text-pretty text-detail-spacebuttom">
        <p>รางวัลที่ได้รับ</p>
        <ul class="list-none dashed list-outside">
          <li>ตั๋วนำโชค 100 รางวัล</li>
        </ul>
      </article>
    </div>
  </div>
</template>

<style>
.div-cover-cardlist {
  @apply sm:px-10 px-4;
}
.div-grid-cover-card {
  @apply lg:gap-4 sm:gap-2 sm:grid;
}
.arrow-bttn-event {
  @apply md:w-6 md:h-6 w-4 h-4 text-gray-800 dark:text-black font-light;
}
.time-date-event {
  @apply text-[#AFAFAF] bg-[#F6F6F6]  md:px-[18px]  px-[10px] py-[4px] rounded-full lg:text-lg sm:text-base text-sm;
}
.bttn-visit-event {
  @apply flex items-center justify-center gap-2 font-bold text-black lg:text-lg sm:text-base text-sm;
}
ul.dashed > li {
  text-indent: -5px;
}
ul.dashed > li:before {
  content: "-";
  text-indent: -5px;
}

li {
  margin-left: 22px;
}

.text-detail-spacebuttom {
  margin-bottom: 12px;
}

.no-reward {
  @apply text-end lg:text-[40px] md:text-[36px] text-[32px];
}
/* large-card */
.large-card-frame {
  @apply border rounded-lg shadow-md text-center p-[14px] h-full text-[#BA792D] font-bold w-full mb-4;
}
.large-card-frame-yellow {
  @apply bg-[linear-gradient(360deg,_#fff_60%,64%,_#FDD835_60%)];
}
.large-card-frame-grey {
  @apply bg-[linear-gradient(360deg,_#fff_60%,64%,_#AAAACE_60%)];
}
.large-card-frame-orange {
  @apply bg-[linear-gradient(360deg,_#fff_60%,64%,_#E88102_60%)];
}
.large-card-img {
  @apply mt-[-16px] h-auto mx-auto;
}

.large-card-text-score {
  @apply text-[#AAAAAA] text-[14px] font-medium;
}
.large-card-score {
  @apply text-[#C96203] lg:text-[40px] md:text-[36px] text-[32px];
}
.large-card-awards {
  @apply text-[#E88102] text-[16px] font-normal;
}
.large-no {
  @apply text-white;
}

/* small-card */
.small-card-frame {
  @apply border rounded-lg shadow-md text-center p-[14px] text-[#BA792D] font-bold w-full h-full mb-4;
}
.small-card-img {
  @apply lg:mt-[-34px] mt-[-16px]  h-auto mx-auto;
}
</style>

<script setup lang="ts">
const cardlist = ref([
  {
    image: "/telephone.png",
    point: "3500",
    rewards: "Iphone 12",
    ticketamount: "+150 coins 5 TICKET",
  },
  {
    image: "/vr.png",
    point: "3200",
    rewards: "VR",
    ticketamount: "+150 TICKET",
  },
  {
    image: "/mousecom.png",
    point: "3000",
    rewards: "Mouse Gaming",
    ticketamount: "",
  },
  {
    image: "/flashdrives.png",
    point: "",
    rewards: "USB 2.0",
    ticketamount: "",
  },
  {
    image: "/coins.png",
    point: "",
    rewards: "150 Coins",
    ticketamount: "",
  },
  {
    image: "/coins.png",
    point: "",
    rewards: "100 Coins",
    ticketamount: "",
  },
  {
    image: "/coupons.png",
    point: "",
    rewards: "5 TICKET",
    ticketamount: "",
  },
]);
</script>
