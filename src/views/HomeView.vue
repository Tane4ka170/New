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
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Kedvesem"
            by="ByeAlex"
            to="/artist"
            image="https://cdn-images.dzcdn.net/images/cover/93c395ff3734e20bbc2f9cb064bc2e2d/0x1900-000000-80-0-0.jpg"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Human"
            by="OneRepublic"
            to="/artist"
            image="https://store.onerepublic.com/cdn/shop/files/1R_OhMyMy_AlbumCover.jpg?v=1686938810"
          />
        </div>
        <div class="xl:w-1/3 w-1/2">
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Sorry Not Sorry"
            by="Demi Lovato"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/en/1/13/Sorry_Not_Sorry_%28Official_Single_Cover%29_by_Demi_Lovato.png"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="The Way You Make Me Feel"
            by="Michael Jackson"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/ru/a/aa/Michael_Jackson_%E2%80%94_The_Way_You_Make_Me_Feel_single_cover.jpg"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="The Moon Is Rising"
            by="Samanta Tīna"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/en/3/3a/The_Moon_Is_Rising.jpg"
          />
        </div>
        <div class="xl:w-1/3 w-1/2">
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Visionary Dream"
            by="Sopho"
            to="/artist"
            image="https://i.discogs.com/4rxAVFSe-3BfWPoSCu_KRnlnM94QGbX2syZiZgps3Dk/rs:fit/g:sm/q:90/h:598/w:600/czM6Ly9kaXNjb2dz/LWRhdGFiYXNlLWlt/YWdlcy9SLTExMjMz/ODY5LTE1MTI5MDUw/NTUtNTc5MS5qcGVn.jpeg"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="willow"
            by="Taylor Swift"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/ru/9/9a/Taylor_Swift_-_Willow.png"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Ride"
            by="twenty one pilots"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/ru/1/19/Twenty_one_pilots_ride_cover.jpg"
          />
        </div>
      </div>

      <div class="px-8 mt-8 min-w-[800px]">
        <div class="text-white text-xl font-semibold inline-block">
          Created for you
        </div>

        <div class="py-3"></div>

        <div class="flex justify-start gap-7">
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Twenty One Pilots, Usher and Sopho"
            to="/artist"
            images="{}"
          />
        </div>
      </div>
    </div>
  </div>
</template>
