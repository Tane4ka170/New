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
  if (route.path == pageUrl.value && icon.value === iconString.value + "-red")
    return;

  if (route.path == pageUrl.value) {
    icon.value = iconString.value + "-red";
  } else {
    icon.value = iconString.value + "-white";
  }
});

const isHover = () => {
  if (icon.value == iconString.value + "-red") {
    icon.value = iconString.value + "-white";
  } else if ((icon.value = iconString.value + "-white")) {
    icon.value = iconString.value + "-red";
  }
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
      class=""
    ></RouterLink>
  </div>
</template>
