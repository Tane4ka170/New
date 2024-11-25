<script setup>
import { RouterView, RouterLink } from "vue-router";
import Magnify from "vue-material-design-icons/Magnify.vue";
import Bell from "vue-material-design-icons/Bell.vue";
import SideMenuItem from "./components/SideMenuItem.vue";
</script>

<template>
  <div
    id="TopNav"
    class="fixed right-0 flex items-center justify-between w-[calc(100%-240px)] h-[56px] border-b border-b-[#1781f0]"
  >
    <div class="flex items-center w-full">
      <Magnify class="pl-6 mt-1 pr-2" fillColor="#fffb08" :size="22" />
      <input
        type="text"
        class="p-1 bg-transparent outline-none font-[400] placeholder-[#b117f0] text-[#fff] w-full max-w-xl"
        placeholder="Search"
      />
    </div>
    <div class="flex items-center pr-10">
      <div class="mr-4 p-1 hover:bg-[#d8f017] rounded-full cursor-pointer">
        <Bell fillColor="#1781f0" :size="20" />
      </div>

      <img
        src="https://img.freepik.com/premium-vector/avatar-icon-circle-male-sign-vector-illustration_276184-170.jpg"
        alt=""
        class="rounded-full w-[33px]"
      />
    </div>
  </div>

  <div
    id="SideNav"
    class="fixed w-[240px] bg-[#b117f0] h-[100vh] border-r[#1781f0]"
  >
    <div class="w-full pl-6 pt-3 cursor-pointer">
      <RouterLink to="/" class="text-[#d8f017]">MusicApp</RouterLink>
    </div>

    <div class="mt-[53px]"></div>

    <SideMenuItem iconString="music" :iconSize="20" pageUrl="/" name="Music" />
    <SideMenuItem
      iconString="podcast"
      :iconSize="20"
      pageUrl="/"
      name="Podcasts"
    />
    <SideMenuItem
      iconString="discover"
      :iconSize="20"
      pageUrl="/"
      name="Explore"
    />
    <SideMenuItem
      iconString="favorite"
      :iconSize="20"
      pageUrl="/"
      name="Favorites"
    />
    <div class="text-[#77b5f6] font-light text-[12px] pl-[62px] mt-[25px]">
      <div class="py-[9px] hover:text-[#d8f017] cursor-pointer">
        Favorite tracks
      </div>
      <div class="py-[9px] hover:text-[#d8f017] cursor-pointer">Playlist</div>
      <div class="py-[9px] hover:text-[#d8f017] cursor-pointer">Albums</div>
      <div class="py-[9px] hover:text-[#d8f017] cursor-pointer">Artists</div>
      <div class="py-[9px] hover:text-[#d8f017] cursor-pointer">Podcasts</div>
    </div>
  </div>

  <div
    class="fixed w-[calc(100%-240px)] h-[calc(100-56px)] ml-[240px] mt-[56px] overflow-x-auto"
  >
    <RouterView />
  </div>
</template>
