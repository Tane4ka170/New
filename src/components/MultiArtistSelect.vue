<script setup>
import { toRefs, ref } from "vue";
import { RouterLink, useRoute } from "vue-router";

import Play from "vue-material-design-icons/Play.vue";

const route = useRoute();
const props = defineProps({
  category: String,
  images: Object,
  text: String,
  to: String,
});
const { by, image, text, to } = toRefs(props);

let isHover = ref(false);
</script>

<template>
  <div>
    <RouterLink :to="to" class="relative">
      <div
        @mouseenter="() => isHover(true)"
        @mouseleave="() => isHover(false)"
        class="flex justify-center items-center contrast-[1] brightness-[0.87] rounded-md aspect-square overflow-hidden"
      >
        <div
          :class="
            isHover
              ? 'transition ease-in duration-150 bg-opacity-20'
              : 'transition ease-out duration-150 bg-opacity-5'
          "
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
            class="absolute contrast-[0.55] right-0 top-0 w-1/2"
          />
          <img
            :src="images.three"
            alt=""
            class="absolute contrast-[0.55] right-0 top-0 w-1/2"
          />
          <img
            :src="images.four"
            alt=""
            class="absolute contrast-[0.55] right-0 top-0 w-1/2"
          />
        </div>
      </div>
    </RouterLink>
  </div>
</template>
