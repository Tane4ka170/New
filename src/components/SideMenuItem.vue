<script setup>
import { toRefs, ref, watchEffect } from "vue";
import { RouterLink, useRoute } from "vue-router";

const route = useRoute();
const props = defineProps({
  iconString: String,
  iconSize: Number,
  pageUrl: String,
  name: String,
});
const { iconString, pageUrl, name } = toRefs(props);

let icon = ref(null);

watchEffect(() => {
  if (route.path === pageUrl.value) {
    icon.value = iconString.value + "-black";
  } else {
    icon.value = iconString.value + "-fill";
  }
});

const isHover = (hovering) => {
  icon.value = hovering
    ? iconString.value + "-fill"
    : iconString.value + "-black";
};
</script>

<template>
  <div class="flex items-center w-full my-[20px]">
    <RouterLink
      :to="pageUrl"
      :class="
        pageUrl === route.path
          ? 'border-l-[#d8f017] text-[#d8f017]'
          : 'border-l-[#1781f0] text-white'
      "
      class="border-l-4 w-full hover:text-[#d8f017]"
      @mouseenter="() => isHover(true)"
      @mouseleave="() => isHover(false)"
    >
      <div class="flex items-center pl-3 mx-3 cursor-pointer">
        <img :src="`/images/icons/${icon}.png`" alt="icon" :width="iconSize" />
        <div class="pl-3.5 font-[600] text-[17px]">{{ name }}</div>
      </div>
    </RouterLink>
  </div>
</template>
