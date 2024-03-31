<template>
  <head>
    <link
      href="https://fonts.googleapis.com/css?family=Kanit"
      rel="stylesheet"
    />
  </head>
  <headbar :amount="'100.00 ฿'" :name="'Usergaming'" />
  <Bigimage :url="'/big-gaming-competition.png'" />
  <div class="bg-blue-800 flex justify-center">
    <div class="text-white flex">
      <Iconsmall
        :url="'/simple-icons_gamemaker.svg'"
        :iconname="'ทัวร์นาเมนต์ทั้งหมด'"
        :imgchange="'/simple-icons_gamemaker-active.png'"
      />
      <Iconsmall
        :url="'/mdi_announcement.svg'"
        :iconname="'ประกาศ'"
        :imgchange="'i-zondicons:announcement'"
      />
      <Iconsmall
        :url="'/material-symbols_rewarded-ads-rounded.svg'"
        :iconname="'ผลรางวัล'"
        :imgchange="'/material-symbols_rewarded-ads-rounded-active.png'"
      />
      <Iconsmall
        :url="'/icon-park-solid_ranking-list.svg'"
        :iconname="'ตารางอันดับ'"
        :imgchange="'i-icon-park-solid:alignment-bottom-center'"
      />
    </div>
  </div>

  <div class="md:container mx-auto lg:px-36">
    <div class="bg-zinc-50 w-full grid gap-y-5">
      <cardlist />
      <Listplayer />
      <notificationbutton
        :no="'จ'"
        :img="'/profile-image.png'"
        :name="'TIGER711R11824'"
        :imgbttn="'รับรางวัล'"
      />
    </div>
  </div>
</template>

<style>
body {
  @apply bg-zinc-300;
  font-family: "Kanit";
}

@import url("https://fonts.googleapis.com/css2?family=Kanit");
.background-blue {
  background-color: #2237a7;
}

.dis-flex {
  display: flex;
}
.center-content {
  align-items: center;
  text-align: center;
  color: #fff;
  padding: 10px;
}
.center-content:hover {
  color: #fdd835;
}
</style>
