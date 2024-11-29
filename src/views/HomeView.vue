<script setup>
import BlendsInfluencedBy from "../components/BlendsInfluencedBy.vue";
import MultiArtistSelect from "../components/MultiArtistSelect.vue";
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
            text="Featuring Katy Perry, Britney Spears and Drax Project"
            to="/artist"
            :images="{
              one: 'https://miro.medium.com/v2/resize:fit:681/1*EBOL4lka5QjcYoxj6AHp-g.png',
              two: 'https://aimm.edu/hubfs/Blog%20Images/Top%2010%20Album%20Covers%20of%202017/Tyler%20the%20Creator-%20Flower%20boy.jpg',
              three:
                'https://upload.wikimedia.org/wikipedia/commons/3/33/Are_You_Experienced_-_US_cover-edit.jpg',
              four: 'https://www.billboard.com/wp-content/uploads/2022/06/beyonce-Lemonade-album-art-billboard-1240.jpg?w=600',
            }"
          />
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Hailee Steinfeld, Little Mix and Nicki Minaj"
            to="/artist"
            :images="{
              one: 'https://www.usatoday.com/gcdn/authoring/authoring-images/2024/04/18/USAT/73369584007-013-1989-taylors-version-2023.jpeg',
              two: 'https://www.skillshare.com/blog/wp-content/uploads/2016/06/ScreenShot2020-10-20at11.36.46AM.png',
              three:
                'https://qodeinteractive.com/magazine/wp-content/uploads/2020/06/16-Tame-Impala.jpg',
              four: 'https://www.sleek-mag.com/wp-content/uploads/2017/05/takashi_murakami_kanye_west.jpg',
            }"
          />
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Dana International, Claudia Pascoal and Beyoncé"
            to="/artist"
            :images="{
              one: 'https://pure-music.co.uk/wp-content/uploads/2019/04/Thriller-Album-Cover.png',
              two: 'https://www.indieground.net/images/blog/2024/indieblog-best-album-covers-2010s-23.jpg',
              three:
                'https://images.theconversation.com/files/512871/original/file-20230301-26-ryosag.jpg?ixlib=rb-4.1.0&rect=97%2C79%2C5799%2C5817&q=45&auto=format&w=926&fit=clip',
              four: 'https://cdn-images.dzcdn.net/images/cover/967ac8605268db88a1e597394115365d/1900x1900-000000-80-0-0.jpg',
            }"
          />
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Raiven, Natalia Barbu and One Direction"
            to="/artist"
            :images="{
              one: 'https://www.billboard.com/wp-content/uploads/media/ariana-grande-sweetner-album-art-2018-billboard-1240.jpg?w=600',
              two: 'https://www.billboard.com/wp-content/uploads/2022/03/48.-Lady-Gaga-%E2%80%98The-Fame-Monster-2009-album-art-billboard-1240.jpg?w=600',
              three:
                'https://www.billboard.com/wp-content/uploads/2023/07/rihanna-anti-cover-2016-billboard-1240.jpg?w=600',
              four: 'https://www.billboard.com/wp-content/uploads/2022/03/35.-Metallica-%E2%80%98Master-of-Puppets-1986-album-art-billboard-1240.jpg?w=600',
            }"
          />
        </div>
      </div>
    </div>
  </div>
</template>
