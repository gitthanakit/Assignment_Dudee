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
      <Iconsmall />
    </div>
  </div>

  <div class="md:container mx-auto xl:px-[200px] lg:px-[80px]">
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
