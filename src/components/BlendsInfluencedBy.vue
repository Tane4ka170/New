<script setup>
import { toRefs, ref } from "vue";
import { RouterLink } from "vue-router";

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
      ></div>
    </RouterLink>
  </div>
</template>
