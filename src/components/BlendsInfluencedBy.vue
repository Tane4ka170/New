<script setup>
import { toRefs, ref } from "vue";
import { RouterLink, useRoute } from "vue-router";

import Play from "vue-material-design-icons/Play.vue";

const route = useRoute();
const props = defineProps({
  by: String,
  image: String,
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
        class="flex items-center bg-[#1781f0] rounded-sm h-[54px] relative"
        @mouseenter="isHover = true"
        @mouseleave="isHover = false"
      >
        <div
          :class="
            isHover
              ? 'transition ease-in duration-100 bg-opacity-40'
              : 'transition ease-out duration-100 bg-opacity-5'
          "
          class="absolute h-full z-10 w-[54px] bg-black rounded-sm"
        >
          <div
            :class="
              isHover
                ? 'transition ease-in duration-100 bg-opacity-1000'
                : 'transition ease-out duration-100 opacity-0'
            "
            class="absolute z-20 p-1.5 rounded-full bg-white left-[6px]"
          >
            <Play :size="30" />
          </div>
          <img src="" alt="" class="min-h-[54px] min-w-[54px] rounded-sm z-0" />
        </div>
      </div>
    </RouterLink>
  </div>
</template>
