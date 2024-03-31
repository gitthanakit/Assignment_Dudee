<template>
  <div class="px-[22px]">
    <div class="flex justify-between pt-[16px] pb-[22px]">
      <div class="flex items-center justify-center gap-2 grid-cols-2">
        <svg
          class="w-6 h-6 text-gray-800 dark:text-black font-light"
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
        <p class="font-bold text-black">ทัวร์นาเมนต์ บี</p>
      </div>
      <div class="text-[#AFAFAF] bg-[#F6F6F6] py-[8px] px-[22px] rounded-full">
        หมดเวลากิจกรรม
      </div>
    </div>
    <div class="px-10">
      <div class="flex items-center justify-center gap-4 grid grid-cols-3">
        <div class="large-card-frame-yellow">
          <p class="large-no">1<sup>th</sup></p>
          <img src="/telephone.png" alt="" class="large-card-img" />
          <p class="large-card-text-score">Score</p>
          <p class="large-card-score">3500</p>
          <p class="large-card-awards">Iphone 12</p>
          <p class="large-card-awards">+150 coins 5 TICKET</p>
        </div>
        <div class="large-card-frame-grey">
          <p class="large-no">2<sup>th</sup></p>
          <img src="/vr.png" alt="" class="large-card-img" />
          <p class="large-card-text-score">Score</p>
          <p class="large-card-score">3200</p>
          <p class="large-card-awards">VR</p>
          <p class="large-card-awards">+150 TICKET</p>
        </div>
        <div class="large-card-frame-orange">
          <p class="large-no">3<sup>th</sup></p>
          <img src="/mousecom.png" alt="" class="large-card-img" />
          <p class="large-card-text-score">Score</p>
          <p class="large-card-score">3000</p>
          <p class="large-card-awards">Mouse Gaming</p>
        </div>
      </div>

      <div class="flex items-center justify-center gap-4 grid grid-cols-4 my-6">
        <div class="small-card-frame">
          <p class="small-card-no">4<sup>th</sup></p>
          <img src="/flashdrives.png" alt="" class="small-card-img" />
          <p>USB 2.0</p>
        </div>

        <div class="small-card-frame">
          <p class="small-card-no">5<sup>th</sup></p>
          <img src="/coins.png" alt="" class="small-card-img" />
          <p class="align-bottom">USB 2.0</p>
        </div>

        <div class="small-card-frame">
          <p class="small-card-no">6<sup>th</sup></p>
          <img src="/coins.png" alt="" class="small-card-img" />
          <p>USB 2.0</p>
        </div>
        <div class="small-card-frame">
          <p class="small-card-no">7<sup>th</sup></p>
          <img src="/coupons.png" alt="" class="small-card-img" />
          <p>USB 2.0</p>
        </div>
      </div>
    </div>
    <div>
      <div class="text-detail-spacebuttom">
        <p>ทัวร์นาเมนต์แข่งขันยอดเล่นเกมออนไลน์</p>
        <p>
          เริ่มกิจกรรมวันที่ 19 มกราคม 2567 สิ้นสุดกิจกรรมและแจกรางวัล วันที่ 29
          มกราคม 2567
        </p>
      </div>
      <div class="text-detail-spacebuttom">
        <p>กติกาการแข่งขัน</p>
        <ol class="list-decimal list-outside">
          <li>แข่งขันยอดเล่นเกมออนไลน์</li>
          <li>แจกรางวัลให้ผู้เล่นที่ได้ลำดับที่ 1, 2, 7</li>
        </ol>
      </div>
      <div class="text-detail-spacebuttom">
        <p>รางวัลที่ได้รับ</p>
        <ul class="list-none dashed list-outside">
          <li>ตั๋วนำโชค 100 รางวัล</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style>
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

/* large-card */
.large-card-frame-yellow {
  @apply border rounded-lg shadow-md text-center p-[14px] h-full text-[#BA792D] font-bold w-full bg-[linear-gradient(360deg,_#fff_60%,64%,_#FDD835_60%)];
}
.large-card-frame-grey {
  @apply border rounded-lg shadow-md text-center p-[14px] h-full text-[#BA792D] font-bold w-full bg-[linear-gradient(360deg,_#fff_60%,64%,_#AAAACE_60%)];
}
.large-card-frame-orange {
  @apply border rounded-lg shadow-md text-center p-[14px] h-full text-[#BA792D] font-bold w-full bg-[linear-gradient(360deg,_#fff_60%,64%,_#E88102_60%)];
}
.large-card-img {
  @apply mt-[-40px] h-auto mx-auto;
}
.large-card-no {
  @apply text-end text-[36px];
}
.large-card-text-score {
  @apply text-[#AAAAAA] text-[14px] font-medium;
}
.large-card-score {
  @apply text-[#C96203] text-[36px];
}
.large-card-awards {
  @apply text-[#E88102] text-[16px] font-normal;
}
.large-no {
  @apply text-end text-white text-[40px];
}

/* small-card */
.small-card-frame {
  @apply border rounded-lg shadow-md text-center p-[14px] text-[#BA792D] font-bold w-full h-full;
}
.small-card-img {
  @apply mt-[-40px] h-auto mx-auto;
}
.small-card-no {
  @apply text-end text-[36px];
}
</style>
