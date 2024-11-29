<script setup>
import { toRefs, ref } from "vue";
import { RouterLink } from "vue-router";
import Play from "vue-material-design-icons/Play.vue";

const props = defineProps({
  category: String,
  images: Object,
  text: String,
  to: String,
});

const { category, images, text, to } = toRefs(props);

let isHover = ref(false);
</script>

<template>
  <div>
    <RouterLink :to="to" class="relative">
      <div
        @mouseenter="isHover = true"
        @mouseleave="isHover = false"
        class="flex justify-center items-center contrast-[2] brightness-[0.87] rounded-md aspect-square overflow-hidden"
      >
        <div
          :class="{
            'transition ease-in duration-150 bg-opacity-20': isHover,
            'transition ease-out duration-150 bg-opacity-5': !isHover,
          }"
          class="absolute w-full h-full bg-black z-10 rounded-md"
        >
          <img
            :src="images.one"
            alt=""
            class="absolute contrast-[0.55] right-0 top-0 w-1/2"
          />
          <img
            :src="images.two"
            alt=""
            class="absolute contrast-[0.55] left-0 top-0 w-1/2"
          />
          <img
            :src="images.three"
            alt=""
            class="absolute contrast-[0.55] right-0 bottom-0 w-1/2"
          />
          <img
            :src="images.four"
            alt=""
            class="absolute contrast-[0.55] left-0 bottom-0 w-1/2"
          />

          <div
            class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 z-20 p-2 rounded-full bg-white inline-block"
          >
            <Play :size="33" />
          </div>

          <div
            class="absolute z-30 flex items-center bottom-1 left-0 h-7 ml-1 bg-black rounded-full px-2 bg-opacity-10"
          >
            <img
              src="/images/logo.png"
              alt=""
              class="pr-2 opacity-[0.75] brightness-[1.2]"
              width="30"
            />
            <div class="text-white font-bold text-[21px]">{{ category }}</div>
          </div>
        </div>
      </div>
    </RouterLink>
    <div class="h-2">
      <RouterLink :to="to">
        <div class="hover:underline text-lime-200 font-light text-sm">
          {{ text }}
        </div>
      </RouterLink>
    </div>
  </div>
</template>
