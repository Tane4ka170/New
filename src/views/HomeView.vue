<script setup>
import BlendsInfluencedBy from "../components/BlendsInfluencedBy.vue";
</script>

<template>
  <div class="max-w-[1500px] mx-auto">
    <div class="px-8 mt-8 min-v-[800px] w-full">
      <div class="text-white text-xl font-semibold inline-block">
        Blends influenced by...
        <div class="text-sm font-normal text-[#1781f0]">
          Find new tracks that match your favorites
        </div>
      </div>

      <div class="py-3"></div>

      <div class="flex justify-between w-full gap-8">
        <div class="xl:w-1/3 w-1/2">
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Only Teardrops"
            by="Emilie de Forest"
            to="/artist"
            image="https://is1-ssl.mzstatic.com/image/thumb/Music2/v4/0c/c8/0f/0cc80f43-d7d1-31b5-724a-8b41b22787de/886443998551.jpg/1200x1200bb.jpg"
          />
        </div>
      </div>
    </div>
  </div>
</template>
